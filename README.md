# 🦄 Pony Diffusion V6 XL - 완전 무검열(Uncensored) 이미지 생성기

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)

Google Colab 무료 환경(T4 GPU)에 최적화된 **완전 무검열(100% Zero Censorship) 이미지 생성 웹 UI**입니다.

14GB에 달하던 기존의 무거운 분할 모델 구조를 제거하고, **단일 6.4GB 올인원(All-in-One) 모델**을 채택하여 **메모리 부족(OOM)이나 멈춤 현상 없이 단 15~20초 만에 이미지를 생성**합니다.

---

## 📌 주요 특징
- **100% 완전 무검열 (Zero Censorship)**: 어떤 검열이나 안전 필터도 없는 순수 오픈 가중치 모델.
- **6.4GB 단일 파일**: 별도의 9GB 텍스트 인코더가 필요 없어 Colab 12.7GB 램 한도 초과 및 멈춤이 원천 방지됩니다.
- **초고속 생성 (15~20초)**: DPM++ 2M Karras 스케줄러를 적용하여 22스텝 만에 초고화질 완성.
- **원클릭 웹 폼**: 복잡한 노드 화면 없이 프롬프트 입력창과 결과 이미지 창만 직관적으로 제공.

---

## 🚀 사용 방법

1. 상단의 **[Open In Colab](https://colab.research.google.com/github/Th3Sign/qwen-image-2.1-colab/blob/main/Qwen_Image_2_1_Serving.ipynb)** 링크를 클릭하여 Colab에서 엽니다.
2. `런타임 > 런타임 유형 변경`에서 **T4 GPU**로 설정되어 있는지 확인합니다.
3. `런타임 > 모두 실행` (`Ctrl + F9`)을 누릅니다.
4. 4단계 셀 아래에 웹 입력창이 열리면 원하는 프롬프트를 적고 **`[🚀 이미지 생성하기]`**를 클릭합니다.
   *(약 15~20초 후 바로 오른쪽에 완성된 이미지가 나타납니다!)*
