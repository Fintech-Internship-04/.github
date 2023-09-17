# Face Your Pace - 카우러너

### 목차

1. [🏃 서비스 소개](#-서비스-소개)
2. [🏃 프로젝트 세부 내용](#-프로젝트-세부-내용)
3. [⏰ 개발 기간](#-개발-기간-20220227--20220610)
4. [✨ 주요기능 소개](#-주요기능-소개)
5. [🛠️ 기술스택](#%EF%B8%8F-기술스택)
6. [✏️ 기획 및 설계](#%EF%B8%8F-기획-및-설계)


# 🏃 서비스 소개

![슬라이드6](https://github.com/Fintech-Internship-04/.github/assets/11494592/42f0ee45-c46a-4a66-9ddb-4f6a3a73930b)
![슬라이드8](https://github.com/Fintech-Internship-04/.github/assets/11494592/a94fa2fc-954b-483e-b9b0-26f9496c6edc)
![슬라이드10](https://github.com/Fintech-Internship-04/.github/assets/11494592/27f1b3e4-6bb8-4bdb-9c00-02589feba69b)
![슬라이드11](https://github.com/Fintech-Internship-04/.github/assets/11494592/6d8970f7-e5b7-4dd6-821f-f7f11065ca89)
![슬라이드12](https://github.com/Fintech-Internship-04/.github/assets/11494592/ad6d3e19-7f8b-4ccb-af4a-c6899d64645d)
![슬라이드13](https://github.com/Fintech-Internship-04/.github/assets/11494592/60879424-951c-4c77-b951-40d7163c59cd)
![슬라이드14](https://github.com/Fintech-Internship-04/.github/assets/11494592/2c0df2fb-c095-4af5-bd49-4250c0cfee66)



### 🌞 프로젝트 동기

  스포츠 심리학 저널에 게재된 영국의 브루넬 대학교(Brunel University) 스포츠 교육학과 코스타스 카라게오그리스(Costas Karageorghis) 박사의 연구 결과에 따르면, 음악을 들으면서 운동하면 평소보다 15% 정도 더 오래 운동을 지속할 수 있다고 한다. 또한 운동할 때 음악을 적절하게 선택하면 신진대사, 근력, 호흡, 심박수 및 혈압 등에 영향을 주며 근육의 반사작용을 일으키게 하여 피로를 잊게 만들어주는 등 운동효과를 높여 준다.

  달리기의 경우, 1km를 얼마나 빠른 속도로 달리는지 측정지표인 ‘페이스(m/km)' 가 있다. 노래를 들으며 달릴 때, 목표로 하는 페이스와 속도가 맞는 노래를 듣는 경우에는 노래를 들으며 박자에 맞게 뛸 수 있지만, 본인의 페이스에 비해 조금 느리거나 빠른 노래가 나오면 운동 리듬 유지에 큰 어려움이 있다.

  사용자의 원하는 속도를 반영하여 노래를 재생시킴으로써 사용자의 운동 페이스를 일정하게 유지하게 한다. 이렇게 리듬을 잃지 않고 운동하게 도와줌으로써 운동 효과를 극대화시킬 수 있는 서비스를 만들게 되었다.

### 🌞 타겟층


1) 술자리 등과 같은 모임 자리에서 자동 정산을 빠르게 하고자 하는 20대에서 30대 청년
2) 모임별 자동 정산 내역을 빠르게 확인하고자 하는 사람

따라서 이 서비스는 모임에서 더치페이를 많이 하는 사람들에게 적합한 서비스입니다.

# 🏃 프로젝트 세부 내용

### ✏️ 프로젝트 구조

#### System Architecture 

![슬라이드46](https://github.com/Fintech-Internship-04/.github/assets/11494592/e553e1fd-2267-4373-b780-f3ce3330bad7)

1. Next.js로 프론트를 구성하고 axios를 통해 Spring boot Rest API를 요청하고 응답
2. Springboot로 개발한 모임 정산, 유저, 계좌 관련 RestFUL API를 호출하여 데이터를 송수신함
3. API 서버와 MySQL DB를 각각 AWS EC2에 배포
4. AWS 서버는 HTTPS 프로토콜이 적용되었음 

### 클라우드 설계 구조
![슬라이드47](https://github.com/Fintech-Internship-04/.github/assets/11494592/c3142c86-30c4-4691-98ca-b8809e5a37b9)

### ✏️ DB 설계

![슬라이드44](https://github.com/Fintech-Internship-04/.github/assets/11494592/f3e5360a-e542-4d02-b5d2-726b155e4996)

### ✏️ 기술 Logic

- 음악 다운로드 및 플레이리스트 생성

<img width="714" alt="다운플리생성" src="https://user-images.githubusercontent.com/56347876/172786023-39ee0e8c-9f82-424a-a9d4-8a61c674241d.png">

- 음원 처리

<img width="704" alt="음원" src="https://user-images.githubusercontent.com/56347876/172786053-b8b32555-1aae-4995-b8d4-48315a1b1bdc.png">

- BPM 추천

<img width="706" alt="bpm" src="https://user-images.githubusercontent.com/56347876/172786045-e3067479-1407-4240-8ace-7257705b06ff.png">


## ⏰ 개발 기간 (2022.0 ~ 2022.06.10)

기획 : 2023.06.22 ~ 2023.08.03    
개발 : 2023.08.05 ~ 2023.08.21


# 🏃 주요기능 소개

### 1️⃣ 로그인, 회원가입

<img width="1617" alt="1 로그인'" src="https://user-images.githubusercontent.com/56347876/172768562-01e41f7d-5760-4100-9453-a981fe719d9d.png">
<img width="1629" alt="2 회원가입" src="https://user-images.githubusercontent.com/56347876/172768607-7948eadc-d902-42ff-b9ed-5fb5a09bb97d.png">
<img width="1162" alt="회원가입222" src="https://user-images.githubusercontent.com/56347876/172796209-2a3881e9-3a88-45e1-807c-5181050db57c.png">

### 🛠️ 기술스택

- FrontEnd   
   - NestJS
   - Vercel

- BackEnd   
    - Springboot
    - MySQL
    - Mybatis

- Cloud
    - AWS EC2
- Collaboration
    - Github

### ✏️ 기획 및 설계

[📌 API 명세서](https://github.com/Fintech-Internship-04/already-FE)

[📌 Github(Frontend)](https://github.com/2022-1-Capstone-Project/face-your-pace-frontend)

[📌 Github(Backend)](https://github.com/Fintech-Internship-04/Fintech-Internship-04-BE)
