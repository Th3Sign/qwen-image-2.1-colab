# Qwen-Image-2.1 Uncensored (GGUF) 원클릭 이미지 생성기

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)

Google Colab 환경에서 **[abenzerps/Qwen-Image-2.1-Uncensored-GGUF](https://huggingface.co/abenzerps/Qwen-Image-2.1-Uncensored-GGUF)** 모델을 **심플 웹 UI (Gradio)**로 원클릭 실행하는 노트북입니다.

복잡한 노드 연결이나 복잡한 설정 없이, **프롬프트 입력창에 원하는 그림 설명만 적고 [생성] 버튼을 누르면 AI가 이미지를 생성**합니다.

---

## 🎨 주요 특징
- **초간단 UI**: 복잡한 ComfyUI 노드 화면 대신, 프롬프트 입력창과 결과 이미지 창만 있는 직관적인 웹 인터페이스 제공.
- **Colab 내부 즉시 렌더링**: Colab 화면 바로 아래에서 바로 입력하고 이미지를 볼 수 있으며, 별도 공유 링크(`gradio.live`)로도 접속 가능.
- **T4 GPU 맞춤 최적화**: Q4_0 양자화 모델 및 INT8 텍스트 인코더로 Colab 무료 T4 GPU에서 메모리 부족(OOM) 없이 안정적 구동.

---

## 🚀 사용 방법

1. 상단의 **[Open In Colab](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)** 배지를 클릭하여 Colab에서 노트북을 엽니다.
2. `런타임 > 런타임 유형 변경`에서 **T4 GPU**로 설정되어 있는지 확인합니다.
3. `런타임 > 모두 실행` (`Ctrl + F9`)을 누릅니다.
4. 마지막 4단계 셀이 실행되면 **Colab 화면 바로 아래에 깔끔한 프롬프트 입력창**이 열립니다!
5. 원하는 설명을 적고 **`[🚀 이미지 생성하기]`**를 누르면 끝납니다.
