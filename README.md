# 🚀 Qwen-Image-2.1 Uncensored (Q4_0 GGUF) - Colab 검증 생성기

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)

Google Colab 환경(T4 GPU)에서 **[Qwen-Image-2.1-Uncensored-GGUF](https://huggingface.co/abenzerps/Qwen-Image-2.1-Uncensored-GGUF)** 모델을 직접 검증할 수 있도록 구성된 **원클릭 웹 폼 생성기**입니다.

복잡한 ComfyUI 노드 화면을 조작할 필요 없이, **프롬프트 입력 폼**만으로 깔끔하게 이미지를 생성하고 품질을 테스트할 수 있습니다.

---

## 📌 구성 모델 사양
- **Diffusion Backbone**: `qwen-image-2.1-UC-Q4_0.gguf` (4.15 GB)
- **Text Encoder**: `qwen3vl_8b_int8_convrot.safetensors` (9.35 GB, INT8 저용량 버전)
- **VAE**: `qwen_image_2.1_vae_bf16.safetensors` (676 MB)
- **Backend Engine**: ComfyUI + ComfyUI-GGUF (`--lowvram` 최적화)
- **Frontend**: Gradio Simple Web Form (프롬프트 입력창 + 원클릭 생성 버튼 + 결과 이미지)

---

## 🚀 사용 방법

1. 상단의 **[Open In Colab](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)** 링크를 클릭하여 Colab 노트북을 엽니다.
2. Colab 상단 메뉴에서 **`런타임` > `런타임 유형 변경`**을 눌러 하드웨어 가속기가 **T4 GPU**로 되어 있는지 확인합니다.
   > **⚠️ 주의**: 이전 실행 중 메모리 누수가 발생했다면 **`런타임` > `세션 다시 시작`**을 먼저 한 번 눌러 VRAM을 초기화해 주세요.
3. **`런타임` > `모두 실행`** (단축키: `Ctrl + F9`)을 클릭합니다.
4. 패키지 설치 및 모델 다운로드가 완료되면, 4단계 셀 아래에 웹 UI가 로드됩니다.
5. 프롬프트를 입력하고 **`[🚀 Qwen-Image 2.1 이미지 생성하기]`**를 클릭합니다.

---

## 💡 생성 시간 및 동작 안내
- **첫 실행 시 모델 로딩**:
  - 모델 총 용량이 약 14.2 GB(텍스트 인코더 9.3GB + 디퓨전 4.1GB)이므로, 첫 이미지 생성 버튼 클릭 시 GPU/RAM으로 가중치를 로드하는 데 **약 1~2분의 대기 시간**이 소요됩니다.
  - 진행 상태 창에 경과 시간이 실시간으로 표시되므로 멈춘 것이 아닙니다.
- **권장 해상도**:
  - 빠른 검증: **`768 x 768`** (약 1.5~2분)
  - 정밀 검증: **`1024 x 1024`** (약 3~4분)
