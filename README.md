# Qwen-Image-2.1 Uncensored (GGUF) Colab Serving

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)

Google Colab 환경에서 **[abenzerps/Qwen-Image-2.1-Uncensored-GGUF](https://huggingface.co/abenzerps/Qwen-Image-2.1-Uncensored-GGUF)**의 `qwen-image-2.1-UC-Q4_0.gguf` 모델을 **ComfyUI + Cloudflare Tunnel**로 원클릭 서빙하는 주피터 노트북입니다.

---

## 📌 주요 특징
- **원클릭 실행**: Colab 상단 메뉴에서 `런타임 > 모두 실행`만 누르면 자동으로 ComfyUI 환경 구축 및 모델 다운로드, 서빙까지 진행됩니다.
- **Q4_0 양자화 모델**: VRAM 절약 및 고속 생성을 위해 4.15GB 크기의 GGUF 모델 사용.
- **저메모리 텍스트 인코더**: 시스템 RAM 오프로딩에 최적화된 INT8 ConvRot 텍스트 인코더 (`qwen3vl_8b_int8_convrot.safetensors`, 약 9.35GB) 채택.
- **ComfyUI-GGUF 지원**: Qwen-Image-2.1을 공식 지원하는 `leejet/ComfyUI-GGUF` 커스텀 노드 자동 설치.
- **무료 외부 접속 URL**: Cloudflare Tunnel을 통해 별도 토큰이나 포트포워딩 없이 브라우저로 접속 가능한 HTTPS URL 자동 생성.

---

## 🚀 빠른 시작

1. 상단의 **[Open In Colab](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)** 배지를 클릭하여 Colab에서 노트북을 엽니다.
2. `런타임 > 런타임 유형 변경`에서 가속기가 **T4 GPU** 이상으로 설정되어 있는지 확인합니다.
3. `런타임 > 모두 실행` (`Ctrl + F9`)을 누릅니다.
4. 마지막 단계에서 출력되는 `https://*.trycloudflare.com` 링크를 클릭하면 브라우저에서 ComfyUI 웹 UI가 실행됩니다.

---

## 💡 모델 정보 및 출처
- **Diffusion Model**: [abenzerps/Qwen-Image-2.1-Uncensored-GGUF](https://huggingface.co/abenzerps/Qwen-Image-2.1-Uncensored-GGUF)
- **Base Model**: [Qwen/Qwen-Image-2.1](https://huggingface.co/Qwen/Qwen-Image-2.1)
- **Text Encoder & VAE**: [Comfy-Org/Qwen-Image-2.1](https://huggingface.co/Comfy-Org/Qwen-Image-2.1)
