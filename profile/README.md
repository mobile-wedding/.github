💒 Mobile Wedding

Mobile Wedding은 결혼 문화를 보다 스마트하고 안전하게 바꾸기 위한 모바일 청첩장 플랫폼입니다.
신랑·신부가 직접 청첩장을 생성하고 공유할 수 있으며, AI 기반 사진 자동 분류, 6자리 초대코드 보안, 기념일 리마인드 알림 등 실용적이고 감성적인 기능을 제공합니다.

✨ 주요 기능
•	📸 AI 기반 사진 자동 분류 및 배치
업로드된 웨딩 사진을 GPT + CLIP 모델로 자동 분석하여, 분위기와 스타일에 맞게 청첩장 내에 배치합니다.
사용자는 복잡한 편집 없이도 감성적인 청첩장을 만들 수 있습니다.
•	🔐 6자리 초대코드 보안 기능
청첩장 링크만으로 접근 가능한 기존 구조의 취약점을 보완하여,
신랑·신부가 직접 설정한 6자리 보안코드를 입력해야 청첩장을 열람할 수 있게 설계했습니다.
스미싱 및 무단 열람을 효과적으로 방지합니다.
•	📅 결혼기념일 리마인드 기능
결혼 후 1주년 기념일에 맞춰
청첩장을 다시 리마인드 메세지로 보내드리는 기능을 제공합니다.
단발성 사용이 아닌, 지속 가능한 플랫폼으로서의 가치를 추구합니다.
•	📤 QR코드/링크 공유 지원
청첩장은 웹 링크 및 QR 코드로 간편하게 공유할 수 있어
모바일 환경에서도 접근성이 뛰어납니다.

🛠️ 기술 스택
•	Frontend: React.js
•	Backend: FastAPI (Python)
•	AI 기능: OpenAI GPT + CLIP 모델 기반
•	DB: MySQL
•	배포: AWS EC2, S3
•	보안: 초대코드 기반 접근 제어

💡 개발 목적

기존 모바일 청첩장의 보안 취약점과 일회성 사용 문제를 보완하고,
AI 기술을 접목해 사용자의 부담을 줄이며 더욱 감성적인 경험을 제공하는 것이 목표입니다.

⸻



## 📋 Table of Contents
- [Demo](#-demo)
- [System Architecture](#-system-architecture)
- [Tech stack](#-tech-stack)
- [ERD](#-erd)
- [API](#-api)
- [Monitoring](#-monitoring)
- [How to Start](#how-to-start)
- [Directory Structure](#-directory-structure)
- [Members](#-members)

<br>



## 🎥 Demo

|**회원가입 페이지**|**로그인 페이지**|
|:-------------------:|:---------:|
|<img width="390" height="220" alt="Login Page" src="https://github.com/user-attachments/assets/8eb36c03-c54a-4ba8-ae88-34141bc80983">|<img width="390" height="220" alt="category Page" src="https://github.com/user-attachments/assets/3efc75ea-d067-4247-bf71-5418aa8d5f46">|
|**홈 페이지**|**홈 페이지**|
|<img width="390" height="220" alt="content Page1" src="https://github.com/user-attachments/assets/cebf9217-f7ba-4f22-bee0-90523399a65e">|<img width="390" height="220" alt="seven ai Page2" src="https://github.com/user-attachments/assets/7f03b87b-0c27-4823-8f3b-36ba4679a91f">|
|**샘플 보기**|**청첩장 만들기**|
|<img width="390" height="220" alt="Conversations Page3" src="https://github.com/user-attachments/assets/f696afbb-bc08-471f-bddb-be1a1255e01f">|<img width="390" height="220" alt="Debate Page" src="https://github.com/user-attachments/assets/6ebc1d3f-c517-4476-8322-0be4c6b6ce91">|
|**청첩장 만들기**|**청첩장 만들기**|
|<img width="390" height="220" alt="report Page" src="https://github.com/user-attachments/assets/ba2bdcb1-0548-4435-a296-dc5a83364a16">|<img width="390" height="220" alt="report list Page" src="https://github.com/user-attachments/assets/81eacebe-9696-4104-9f60-159df87d5646">|
|**보안화면**|**완성된 청첩장**|
|<img width="390" height="220" alt="report Page" src="https://github.com/user-attachments/assets/146180a2-7507-4183-b861-1a5a12357cc6">|<img width="390" height="220" alt="report list Page" src="https://github.com/user-attachments/assets/72b8979e-bcb3-4173-a490-f465e0e8cbaf">|
|**완성된 청첩장**|**완성된 청첩장**|
|<img width="390" height="220" alt="report Page" src="https://github.com/user-attachments/assets/d4e60ee1-bd7c-42d5-b488-e8a35274e19b">|<img width="390" height="220" alt="report list Page" src="https://github.com/user-attachments/assets/f45a699a-8a3b-4fb5-903c-d754089f6285">|
|**완성된 청첩장**|
|<img width="390" height="220" alt="report Page" src="https://github.com/user-attachments/assets/1dcaef60-b113-4557-9edd-783af2c1f625">

<br>




## 📍 System Architecture

<img width="1034" alt="image" src="https://github.com/user-attachments/assets/efbac01f-9132-4554-adca-3d178d5155cf" />



## 🛠 Tech stack
<br>
<div align =center>

분야| 사용 기술|
:--------:|:------------------------------:|
**Frontend** |<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black"> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white"> <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white">
**Backend**  |<img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi"> <img src="https://img.shields.io/badge/Uvicorn-22C3E6?style=for-the-badge&logo=uvicorn&logoColor=white"> <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <img src="https://img.shields.io/badge/Claud-D97757?style=for-the-badge&logo=CLIP&logoColor=black"> <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">
**etc** |![Slack](https://img.shields.io/static/v1?style=for-the-badge&message=Slack&color=1E8CBE&logo=Slack&logoColor=FFFFFF&label=) ![Notion](https://img.shields.io/static/v1?style=for-the-badge&message=Notion&color=000000&logo=Notion&logoColor=FFFFFF&label=) ![Figma](https://img.shields.io/static/v1?style=for-the-badge&message=Figma&color=F24E1E&logo=Figma&logoColor=FFFFFF&label=) <img src="https://img.shields.io/badge/swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black">

</div>

## 🎨 ERD
<img width="1290" height="500" alt="Datebase" src="https://github.com/user-attachments/assets/929db8d9-b7a4-4e0d-b8bf-f798dff74fda">

## 💻 API
![image](https://github.com/user-attachments/assets/a73f6dd0-3312-4cab-bead-b1e83409a401)
![image](https://github.com/user-attachments/assets/2b7e9058-9a56-4d69-9f15-e680e768062e)



## How to Start


### Backend
```
git clone https://github.com/mobile-wedding/Wedding-Backend.git
```

### env setting in the Backend folder
app/.env

```
MYSQL_HOST=
MYSQL_PORT=
MYSQL_DB=
MYSQL_PASSWORD=
MYSQL_ROOT_PASSWORD=
MYSQL_USER=


AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=
AWS_S3_BUCKET_NAME=

OPENAI_API_KEY=

EMAIL_ADDRESS=
EMAIL_PASSWORD=
EMAIL_HOST=
EMAIL_PORT=

```

### Run Docker
```
docker-compose up -d --build
```

### Frontend
```
https://github.com/mobile-wedding/Wedding-Frontend.git
```

```
npm i
npm run dev
```

## 📚 Directory Structure

<details>
  <summary><b>Frontend</b></summary>
    <pre>
      <code>
📦 Wedding-Frontend
┣ 📂 public
┃ ┣ 📂 cards
┃ ┃ ┣ 📜 card1_1.png
┃ ┃ ┣ 📜 card1_2.png
┃ ┃ ┣ 📜 card1_3.png
┃ ┃ ┣ 📜 card1_4.png
┃ ┃ ┣ 📜 card1.png
┃ ┃ ┣ 📜 card2.png
┃ ┃ ┣ 📜 card3.png
┃ ┃ ┣ 📜 phone-left.png
┃ ┃ ┗ 📜 phone-right.png
┃ ┗ 📜 vite.svg
┣ 📂 src
┃ ┣ 📂 assets
┃ ┃ ┗ 📜 react.svg
┃ ┣ 📂 components
┃ ┃ ┗ 📜 MapEmbed.jsx
┃ ┣ 📂 pages
┃ ┃ ┣ 📜 Home.css
┃ ┃ ┣ 📜 Home.jsx
┃ ┃ ┣ 📜 Invitation.css
┃ ┃ ┣ 📜 Invitation.jsx
┃ ┃ ┣ 📜 InvitationDetail.css
┃ ┃ ┣ 📜 InvitationDetail.jsx
┃ ┃ ┣ 📜 InvitationPreview.jsx
┃ ┃ ┣ 📜 InvitationSecurity.css
┃ ┃ ┣ 📜 InvitationSecurity.jsx
┃ ┃ ┣ 📜 Login.css
┃ ┃ ┣ 📜 Login.jsx
┃ ┃ ┣ 📜 SignUp.css
┃ ┃ ┗ 📜 SignUp.jsx
┃ ┣ 📜 App.jsx
┃ ┗ 📜 main.jsx
┣ 📜 .env
┣ 📜 .gitignore
┣ 📜 dist.zip
┣ 📜 eslint.config.js
┣ 📜 index.html
┣ 📜 package-lock.json
┣ 📜 package.json
┣ 📜 README.md
┗ 📜 vite.config.js
      </code>
    </pre>
</details>


<details>
  <summary><b>Backend</b></summary>
    <pre>
      <code>
📦 Wedding-Backend
┣ 📂 app
┃ ┣ 📂 crud
┃ ┃ ┣ 📜 anniversary.py
┃ ┃ ┣ 📜 invitation.py
┃ ┃ ┣ 📜 photo.py
┃ ┃ ┗ 📜 user.py
┃ ┣ 📂 routers
┃ ┃ ┣ 📜 anniversary.py
┃ ┃ ┣ 📜 classify.py
┃ ┃ ┣ 📜 invitation.py
┃ ┃ ┣ 📜 layout.py
┃ ┃ ┣ 📜 photo.py
┃ ┃ ┗ 📜 user.py
┃ ┣ 📂 schemas
┃ ┃ ┣ 📜 __init__.py
┃ ┃ ┣ 📜 anniversary.py
┃ ┃ ┣ 📜 invitation.py
┃ ┃ ┣ 📜 photo.py
┃ ┃ ┗ 📜 user.py
┃ ┣ 📂 service
┃ ┃ ┣ 📜 classify.py
┃ ┃ ┗ 📜 layout.py
┃ ┗ 📂 utils
┃ ┃ ┣ 📜 anniversary.py
┃ ┃ ┣ 📜 clip_model.py
┃ ┃ ┣ 📜 gpt_model.py
┃ ┃ ┣ 📜 mailer.py
┃ ┃ ┣ 📜 models.py
┃ ┃ ┣ 📜 s3.py
┃ ┃ ┣ 📜 security.py
┃ ┃ ┗ 📜 send_anniversary.py
┣ 📜 database.py
┣ 📜 main.py
┣ 📜 .env
┣ 📜 .gitignore
┣ 📜 docker-compose.yml
┣ 📜 dockerfile
┣ 📜 README.md
┗ 📜 requirements.txt

      </code>
    </pre>
</details>

## 👑 Members
<table width="100%" align="center" style="border-collapse: collapse; text-align: center;">
<thead>
<tr>
<th>Profiles</th>
<td width="100" align="center">
<a href="https://github.com/bumjpark">
<img src="https://github.com/user-attachments/assets/00b84bdc-cd1a-4fa5-b619-e0fe899d1a09" width="120" height="160">
</a>
</td>


<th>Name</th>
<td width="100" align="center">박종범</td>
</tr>
<th>Position</th>
<td width="150" height="20" align="center">
Backend<br>
Frontend<br>
</td>


