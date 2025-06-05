# 🛍️ 상품 설명 자동화 AI

> 개별 프로젝트

- 프로젝트명 : 상품 설명 자동화 AI (인원 1명)
- 기간 : 2025.05.26 ~ 2025.06.06 (2주)  # 실제 기간으로 수정해주세요.
- Language : Python [3.10.9]  # 실제 Python 버전으로 수정해주세요. (예: Python 3.9)
- Framework : FastAPI [0.115.12]
- 프로젝트 소개 : LLM(거대 언어 모델)을 활용하여 상품 설명을 자동으로 생성하는 AI입니다. 판매자가 효율적으로 상품 설명을 작성하고 마케팅 효과를 높일 수 있도록 돕습니다.

<div align=center>
  <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">    <img src="https://img.shields.io/badge/Hugging_Face-FFD43B?style=for-the-badge&logo=huggingface&logoColor=black">   <img src="https://img.shields.io/badge/flask-000000?style=for-the-badge&logo=flask&logoColor=white"> </div>
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
[2. 주요 기능 및 흐름](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#2-주요-기능-및-흐름)<br>  [3. 기술 스택 및 개발 환경](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#3-기술-스택-및-개발-환경)<br> [4. 모델 학습 및 평가](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#4-모델-학습-및-평가)<br> [5. 웹 인터페이스 구현](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#5-웹-인터페이스-구현)<br> [6. 설치 및 실행 방법](https://github.com/사용자이름/저장소이름?tab=readme-ov-file#6-설치-및-실행-방법)<br> [7. 연구 결과, 시사점 및 개선 방안](#7-연구-결과-시사점-및-개선-방안)<br>

---

## 1. 주제선정 및 배경, 목표

(여기에 프로젝트의 주제 선정 배경과 목표에 대한 설명을 이미지와 함께 추가합니다. "영화 개봉 계절 예측기"와 같은 형식의 이미지 내용이 있다면 좋습니다.)

![주제 및 선정 배경 이미지](https://github.com/user-attachments/assets/주제_배경_이미지_경로.png) ![목표 이미지](https://github.com/user-attachments/assets/목표_이미지_경로.png) ## 2. 주요 기능 및 흐름

(여기에 '상품 설명 자동화 AI'의 주요 기능들과 전체적인 시스템 흐름을 설명하는 이미지나 텍스트를 추가합니다. 예를 들어, 사용자가 키워드를 입력하면 LLM을 통해 설명이 생성되고 웹에 표시되는 과정 등을 설명할 수 있습니다.)

* **키워드 기반 상품 설명 자동 생성:** 사용자가 입력한 핵심 키워드를 바탕으로 AI가 상품 설명을 생성합니다.
* **다양한 상품 카테고리 지원:** 의류, 가전, 식품 등 여러 상품 카테고리에 맞는 맞춤형 설명을 생성할 수 있습니다.
* **생성된 설명 편집 및 저장 기능:** 생성된 설명을 사용자가 직접 수정하고 저장할 수 있는 기능을 제공합니다.

![주요 기능 흐름 이미지](https://github.com/user-attachments/assets/기능_흐름_이미지_경로.png) ## 3. 기술 스택 및 개발 환경

(여기에 프로젝트 개발에 사용된 구체적인 개발 환경, 도구, 라이브러리 버전을 설명합니다. '영화 개봉 계절 예측기'의 '진행 과정, 개발 환경'과 같은 이미지나 텍스트 형식으로 구성할 수 있습니다.)

![기술 스택 상세 이미지](https://github.com/user-attachments/assets/기술_스택_이미지_경로.png) ![개발 환경 상세 이미지](https://github.com/user-attachments/assets/개발_환경_이미지_경로.png) ## 4. 모델 학습 및 평가

(여기에 LLM을 어떻게 활용했는지, 전처리 과정, 모델 학습 과정, 성능 평가 결과 등을 설명하는 이미지나 텍스트를 추가합니다.)

* **데이터 준비**: LLM 학습/활용을 위한 데이터셋 구성 (예: 상품 정보, 기존 상품 설명 등)
* **프롬프트 엔지니어링 / 파인튜닝**: LLM이 효과적으로 상품 설명을 생성하도록 프롬프트 구성 또는 파인튜닝 방법
* **성능 평가**: 생성된 상품 설명의 품질 평가 (정량적/정성적 지표)

![데이터 전처리 이미지](https://github.com/user-attachments/assets/전처리_이미지_경로.png) ![모델 학습 이미지](https://github.com/user-attachments/assets/모델_학습_이미지_경로.png) ![모델 평가 이미지](https://github.com/user-attachments/assets/모델_평가_이미지_경로.png) ## 5. 웹 인터페이스 구현

(여기에는 FastAPI를 사용하여 API를 구축하고, HTML/CSS/JavaScript로 사용자 인터페이스를 어떻게 구현했는지 설명합니다. 스크린샷이나 UI/UX 관련 이미지를 추가하면 좋습니다.)

![웹 인터페이스 이미지](https://github.com/user-attachments/assets/웹_인터페이스_이미지_경로.png) ## 6. 설치 및 실행 방법

프로젝트를 로컬 환경에서 설치하고 실행하는 방법은 다음과 같습니다.

1.  **레포지토리 클론:**
    ```bash
    git clone [https://github.com/yeonhwa88/상품설명AI프로젝트.git](https://github.com/yeonhwa88/상품설명AI프로젝트.git) # 실제 레포지토리 URL로 변경해주세요.
    cd 상품설명AI프로젝트
    ```

2.  **가상 환경 설정 (권장):**
    ```bash
    python -m venv venv
    # Windows
    .\venv\Scripts\activate
    # macOS/Linux
    source venv/bin/activate
    ```

3.  **의존성 설치:**
    ```bash
    pip install -r requirements.txt
    ```
    (만약 `requirements.txt` 파일이 없다면, `pip freeze > requirements.txt` 명령어로 생성하거나, `pip install flask transformers torch` 등 필요한 라이브러리를 직접 설치해주세요.)

4.  **환경 변수 설정 (필요시):**
    * LLM API 키 등이 필요하다면, `.env` 파일을 생성하고 다음과 같이 설정합니다.
        ```
        OPENAI_API_KEY=YOUR_API_KEY # OpenAI 등 특정 LLM API를 사용하는 경우
        ```
    * `python-dotenv` 라이브러리를 사용하여 `.env` 파일을 로드합니다.

5.  **애플리케이션 실행:**
    ```bash
    uvicorn main:app --reload --port 8000 # FastAPI 사용 시
    # 또는 python app.py (Flask 등 다른 프레임워크 사용 시 진입점 파일명으로 변경)
    ```

6.  **접속:**
    애플리케이션이 성공적으로 실행되면, 웹 브라우저를 열고 다음 주소로 접속합니다.
    `http://127.0.0.1:8000` (또는 터미널에 표시되는 주소)

## 7. 연구 결과, 시사점 및 개선 방안

(여기에 프로젝트를 통해 얻은 주요 결과, 이 프로젝트가 가지는 시사점, 그리고 앞으로 개선할 수 있는 방안들을 설명합니다. '영화 개봉 계절 예측기'의 '연구결과, 시사점및개선방안'과 같은 이미지나 텍스트 형식으로 구성할 수 있습니다.)

![연구 결과 이미지](https://github.com/user-attachments/assets/연구_결과_이미지_경로.png) ![시사점 및 개선 방안 이미지](https://github.com/user-attachments/assets/시사점_개선_방안_이미지_경로.png) ---

### 📝 라이선스 (추가 제안)

이 프로젝트는 [MIT License](LICENSE)를 따릅니다. 자세한 내용은 `LICENSE` 파일을 참조하십시오.
*(GitHub에서 레포지토리 생성 시 라이선스를 선택했다면 자동으로 `LICENSE` 파일이 생성됩니다. 아니라면 프로젝트에 `LICENSE` 파일을 추가하는 것을 권장합니다.)*

### ✉️ 문의 (추가 제안)

궁금한 점이 있거나 피드백이 있다면 아래 연락처로 문의해주세요.

* **개발자:** [yeonhwa88](https://github.com/yeonhwa88)
* **이메일:** your_email@example.com (선택 사항)