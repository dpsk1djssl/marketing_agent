
### "내 가게를 살리는 AI 비밀상담사 - 가맹점별 찰떡 마케팅 전략을 찾아라"


## 로컬 개발 환경 구성 방법

```bash
# On macOS and Linux.
# git소스 복사하기
git clone https://github.com/dpsk1djssl/marketing_agent
cd marketing_agent

# venv 환경 설정 (사전에 uv 설치가 필요합니다. 아래 항목 참조)
uv venv
source .venv/bin/activate

# 필요한 python library 설치
uv pip install -r requirements.txt

# streamlit 환경 변수 저장용 폴더 생성 + GOOGLE_API_KEY환경 변수 파일 생성
# (Google API KEY)는 Google AI Studio에서 무료로 생성 가능 (아래 항목 참조)
mkdir .streamlit
echo 'GOOGLE_API_KEY="(Google API KEY)"' > .streamlit/secrets.toml

# 로컬에서 실행
uv run streamlit run streamlit_app.py
```

```bat
:: On Windows
:: git 소스 복사하기
git clone https://github.com/dpsk1djssl/marketing_agent
cd marketing_agent

:: venv 환경 설정 (사전에 uv 설치가 필요합니다. 아래 항목 참조)
uv venv
call .venv\Scripts\activate.bat

:: 필요한 python library 설치
uv pip install -r requirements.txt

:: streamlit 환경 변수 저장용 폴더 생성 + GOOGLE_API_KEY 환경 변수 파일 생성
:: (Google API KEY)는 Google AI Studio에서 무료로 생성 가능 (아래 항목 참조)
mkdir .streamlit
echo GOOGLE_API_KEY="(Google API KEY)" > .streamlit\secrets.toml

:: 로컬에서 실행
uv run streamlit run streamlit_app.py
```

<br>

## uv 설치 방법

https://docs.astral.sh/uv/getting-started/installation/ (공식 사이트. OS에 맞게 설치하면 됩니다.)

<br>

## Google AI Studio API KEY 생성 방법

https://aistudio.google.com/apikey 접속 후 (Google 로그인 필요) Get API KEY 메뉴에서 생성하면 됩니다.
