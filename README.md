# 🛍️ 상품 설명 자동화 AI

> 개별 프로젝트

- 프로젝트명 : 상품 설명 자동화 AI (인원 1명)
- 기간 : [프로젝트 시작일] ~ [프로젝트 종료일] ([기간]주)  # 실제 기간으로 수정
- Language : Python 3.10.9
- Framework : FastAPI 0.115.7, Jinja2 3.1.5, Python-Multipart 0.0.20, uvicorn 0.34.0
- 프로젝트 소개 : LLM(거대 언어 모델)을 활용하여 매력적인 상품 설명을 자동으로 생성, 판매자의 효율성 증대 및 마케팅 효과를 극대화하는 AI 서비스입니다.

<div align=center>
  <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white">   <img src="https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white">
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
[1. 주제선정 및 배경, 목표](#1-주제선정-및-배경-목표)<br>
[2. 주요 기능 및 흐름](#2-주요-기능-및-흐름)<br>
[3. 기술 스택 및 개발 환경](#3-기술-스택-및-개발-환경)<br>
[4. LLM 활용 전략 및 결과물 평가](#4-llm-활용-전략-및-결과물-평가)<br>
[5. 웹 인터페이스 구현](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#5-웹-인터페이스-구현)<br>
[6. 설치 및 실행 방법](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#6-설치-및-실행-방법)<br>
[7. 연구 결과, 시사점 및 개선 방안](#7-연구-결과-시사점-및-개선-방안)<br>

---

### **1. 주제 선정 및 배경, 목표**

이커머스 시장에서 판매자의 효율적인 상품 설명 작성에 대한 어려움에 주목했습니다. 본 프로젝트는 LLM을 활용하여 이 과정을 자동화하고, 판매자의 생산성 및 마케팅 효과를 높이는 것을 목표로 합니다.

### **2. 주요 기능 및 흐름**

* **키워드 기반 상품 설명 자동 생성:** AI가 핵심 키워드를 바탕으로 설명을 생성합니다.
* **다양한 상품 카테고리 지원:** 카테고리별 맞춤형 설명을 생성합니다.
* **생성된 설명 편집 및 저장 기능:** 생성된 설명을 수정하고 저장할 수 있습니다.

### **3. 기술 스택 및 개발 환경**

* **Language:** Python `3.10.9`
* **Core AI:** Google Gemini API (`google-generativeai``gemini-1.5-flash-latest` 라이브러리 활용)
* **Web Framework:** FastAPI `0.115.7`, Jinja2 `3.1.5`, Python-Multipart `0.0.20`, uvicorn `0.34.0`
* **Frontend:** HTML5, CSS3, JavaScript, jQuery, Bootstrap
* **OS/IDE:** Windows10, Jupyter Notebook, VS Code

### **4. LLM 활용 전략 및 결과물 평가**

Google Gemini API를 활용하여 **프롬프트 엔지니어링**으로 상품 설명을 생성했습니다. 유창성, 관련성, 매력성 등 **정성적 기준**과 **사용자 피드백**을 통해 생성된 설명의 품질을 평가했습니다.

### **5. 웹 인터페이스 구현**

사용자가 LLM 기반 상품 설명을 생성하고 활용하도록 직관적인 웹 인터페이스를 구축했습니다.
* **백엔드 API:** `FastAPI`
* **프론트엔드:** `HTML5`, `CSS3`, `JavaScript`, `jQuery`, `Bootstrap` (반응형 디자인 적용)

### **6. 설치 및 실행 방법**

(로컬 환경에서 프로젝트를 실행하기 위한 단계별 가이드입니다.

1.  **레포지토리 클론:**
    ```bash
    git clone https://github.com/yeonhwa88/3rdPersonalProject.git
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
    (Gemini API 키는 Google AI Studio에서 발급받을 수 있습니다.)
5.  **애플리케이션 실행:**
    ```bash
    uvicorn main:app --reload --port 8000
    ```
6.  **접속:**
    웹 브라우저에서 `http://127.0.0.1:8000` (또는 터미널에 표시되는 주소)으로 접속합니다.

### **7. 연구 결과, 시사점 및 개선 방안 📈**

LLM 기반 상품 설명 자동화 시스템 구현으로 **생산성 향상 가능성을 확인**했습니다. 
**프롬프트 엔지니어링의 중요성**을 깨달았으며, 향후 **설명 품질 고도화, 기능 확장(다국어/이미지 기반), SEO 최적화** 등을 통해 개선할 계획입니다.

![연구 결과 이미지](https://github.com/user-attachments/assets/연구_결과_이미지_경로.png) ![시사점 및 개선 방안 이미지](https://github.com/user-attachments/assets/시사점_개선_방안_이미지_경로.png) ---

* **개발자:** [yeonhwa88](https://github.com/yeonhwa88)
