# 상품 설명 자동 생성기

> 개별 프로젝트

- 프로젝트명 : 상품 설명 자동화 AI (인원 1명)
- 기간 : 2025.05.26 ~ 2025.06.06 (1주)
- Language : Python 3.10.9
- Framework : FastAPI 0.115.7, Jinja2 3.1.5, Python-Multipart 0.0.20, uvicorn 0.34.0
- 프로젝트 소개 : LLM(거대 언어 모델)을 활용하여 매력적인 상품 설명을 자동으로 생성, 판매자의 효율성 증대 및 마케팅 효과를 극대화하는 AI 서비스입니다.

<div align=center>
  <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white">   <img src="https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white">
</div>
<div align=center>
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white">
</div>

![깃허브 스택](https://github-readme-stats.vercel.app/api?username=yeonhwa88&show_icons=true&theme=shadow_green)
![깃허브 언어 사용 순위](https://github-readme-stats.vercel.app/api/top-langs/?username=yeonhwa88&layout=compact&theme=dark)

## 목차
[1. 주제 선정 및 배경, 목표](#1-주제-선정-및-배경-목표)<br>
[2. 주요 기능 및 흐름](#2-주요-기능-및-흐름)<br>
[3. 기술 스택 및 개발 환경](#3-기술-스택-및-개발-환경)<br>
[4. LLM 활용 전략 및 결과물 평가](#4-llm-활용-전략-및-결과물-평가)<br>
[5. 웹 인터페이스 구현](#5-웹-인터페이스-구현)<br>
[6. 설치 및 실행 방법](#6-설치-및-실행-방법)<br>
[7. 연구 결과, 시사점 및 개선 방안](#7-연구-결과-시사점-및-개선-방안)<br>

### **1. 주제 선정 및 배경, 목표**

* **이커머스 시장에서 판매자의 효율적인 상품 설명 작성에 대한 어려움에 주목했습니다.** 본 프로젝트는 **Google Gemini와 같은 LLM을 활용**하여 상품 설명 작성 과정을 자동화하고, 판매자의 생산성 및 마케팅 효과를 높이는 것을 목표로 합니다. 수동 작업의 반복을 줄이고, 일관되고 매력적인 설명을 대량으로 생성하는 데 중점을 두었습니다.

### **2. 주요 기능 및 흐름**

* **키워드 기반 상품 설명 자동 생성:** 사용자가 입력한 상품명과 핵심 키워드를 바탕으로 AI(LLM)가 매력적인 상품 설명을 자동으로 생성합니다.
* **정교한 프롬프트 엔지니어링:** LLM이 주어진 제약 조건(예: 300자 이내, 특정 톤앤매너)을 준수하면서도 자연스럽고 설득력 있는 설명을 생성하도록 프롬프트를 설계했습니다.
* **사용자 친화적 인터페이스:** FastAPI 백엔드와 HTML/CSS/JS 프론트엔드를 통해 사용자가 손쉽게 키워드를 입력하고 생성된 설명을 확인할 수 있는 웹 환경을 제공합니다.
* **생성된 설명 활용 및 재시도 기능:** 생성된 설명을 즉시 확인하고, 마음에 들지 않을 경우 '다시 생성하기'를 통해 다른 설명을 얻을 수 있습니다.

### **3. 기술 스택 및 개발 환경**

* **Language:** Python `3.10.9`
* **Core AI:** Google Gemini API (`google-generativeai` 라이브러리 활용, `gemini-1.5-flash-latest` 모델 사용)
    * `dotenv` 라이브러리를 통해 API 키를 안전하게 관리
* **Web Framework:** FastAPI `0.115.7`, Jinja2 `3.1.5`, Python-Multipart `0.0.20`, uvicorn `0.34.0`
* **Frontend:** HTML5, CSS3, JavaScript, jQuery, Bootstrap (반응형 디자인 적용)
* **OS/IDE:** Windows 10, Jupyter Notebook, VS Code

### **4. LLM 활용 전략 및 결과물 평가**

본 프로젝트의 핵심은 **Google Gemini API를 활용한 프롬프트 엔지니어링**입니다.

* **LLM 모델 선택**: Google의 `gemini-1.5-flash-latest` 모델을 사용하여 신속하고 효율적인 텍스트 생성을 목표로 했습니다. 이 모델은 다양한 종류의 텍스트 생성에 적합하며, 특히 짧고 매력적인 상품 설명을 만드는 데 강점을 보였습니다.
* **프롬프트 설계**:
    * **입력 변수**: 사용자가 입력하는 `상품명`과 `키워드`를 LLM의 프롬프트에 동적으로 삽입하여 특정 상품에 대한 맞춤형 설명을 유도했습니다.
    * **명확한 지시**: "마케팅용 상품 설명을 300자 이내로 작성해달라", "자연스럽고 설득력 있는 문장을 사용해달라" 등 LLM이 따라야 할 구체적인 지시사항을 포함했습니다.
    * **역할 부여**: LLM에게 '숙련된 카피라이터'와 같은 역할을 부여하여 결과물의 전문성과 톤앤매너를 향상시켰습니다.
    * **출력 형식 제어**: 생성된 텍스트에서 불필요한 서문이나 맺음말 없이 오직 상품 설명 본문만을 추출하도록 지시했습니다.
* **결과물 평가**:
    * **정성적 기준**: LLM이 생성한 설명의 유창성, 입력 키워드와의 관련성, 독자를 사로잡는 매력성 등을 종합적으로 평가했습니다.
    * **사용자 피드백**: 실제 사용자의 피드백을 통해 생성된 설명이 마케팅 목표에 얼마나 부합하는지, 자연스러운지 등을 검증하고 프롬프트 개선에 활용했습니다.
    * **반복적 개선**: 초기 프롬프트에서 도출된 문제점(예: 너무 짧거나 길거나, 어색한 표현)을 바탕으로 프롬프트를 지속적으로 수정하고 테스트하여 설명의 품질을 고도화했습니다.

### **5. 웹 인터페이스 구현**

사용자가 LLM 기반 상품 설명을 생성하고 활용하도록 직관적인 웹 인터페이스를 구축했습니다.

* **백엔드 API:** `FastAPI`를 활용하여 사용자 요청(상품명, 키워드)을 받아 LLM API를 호출하고, 그 결과를 프론트엔드로 전달하는 RESTful API를 구현했습니다. 비동기 처리를 통해 응답 속도를 최적화했습니다.
* **프론트엔드:** `HTML5`, `CSS3`, `JavaScript`, `jQuery`, `Bootstrap`을 사용하여 사용자가 쉽게 정보를 입력하고 생성된 설명을 시각적으로 확인할 수 있는 반응형 웹 페이지를 개발했습니다. 특히 `Jinja2` 템플릿 엔진을 활용하여 동적인 웹 페이지 렌더링을 구현했습니다.

### **6. 설치 및 실행 방법**

(로컬 환경에서 프로젝트를 실행하기 위한 단계별 가이드입니다.)

1.  **레포지토리 클론:**
    ```bash
    git clone [https://github.com/yeonhwa88/3rdPersonalProject.git](https://github.com/yeonhwa88/3rdPersonalProject.git)
    cd 3rdPersonalProject
    ```
2.  **가상 환경 설정 및 활성화 (권장):**
    ```bash
    python -m venv venv
    .\venv\Scripts\activate # Windows
    # source venv/bin/activate # macOS/Linux
    ```
3.  **의존성 설치:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **환경 변수 설정 (필수):**
    `main.py` 파일과 같은 위치에 `.env` 파일을 생성하고, Gemini API 키를 다음과 같이 추가합니다.
    ```
    GOOGLE_API_KEY="YOUR_GEMINI_API_KEY"
    ```
    (Gemini API 키는 [Google AI Studio](https://aistudio.google.com/app/apikey)에서 발급받을 수 있습니다.)

5.  **애플리케이션 실행:**
    ```bash
    uvicorn main:app --reload --port 8000
    ```
6.  **접속:**
    웹 브라우저에서 `http://127.0.0.1:8000` (또는 터미널에 표시되는 주소)으로 접속합니다.

### **7. 연구 결과, 시사점 및 개선 방안 📈**

* 본 프로젝트를 통해 LLM 기반 상품 설명 자동화 시스템 구현으로 **판매 업무의 생산성 향상 가능성**을 명확히 확인했습니다.
* 특히, 원하는 품질의 결과물을 얻기 위한 **프롬프트 엔지니어링의 중요성**을 깊이 이해하게 되었습니다. LLM의 성능을 극대화하기 위해서는 입력 프롬프트의 설계가 핵심적인 요소임을 깨달았습니다.
* 향후 **설명 품질 고도화**(더욱 다양한 톤앤매너, 타겟 고객층별 맞춤형 설명), **기능 확장**(이미지 기반 상품 특징 추출, 다국어 번역 지원), **SEO 최적화**를 위한 키워드 추천 기능 등을 통해 서비스를 개선하고 발전시킬 계획입니다.


* **개발자:** [yeonhwa88](https://github.com/yeonhwa88)