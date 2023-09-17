# 어 벌써? - 뿜빠야

### 목차

1. [🏃 서비스 소개](#-서비스-소개)
2. [🏃 프로젝트 세부 내용](#-프로젝트-세부-내용)
3. [⏰ 개발 기간](#-개발-기간-20220227--20220610)
4. [✨ 주요기능 소개](#-주요기능-소개)
5. [🛠️ 기술스택](#%EF%B8%8F-기술스택)
6. [✏️ 기획 및 설계](#%EF%B8%8F-기획-및-설계)


# 🏃 서비스 소개



### 🌞 프로젝트 동기

술자리, 회식 등 모임에 참석하는 사람들이 많으며 이에 따라 더치페이를 해야 할 상황이 많이 발생합니다.  

![슬라이드6](https://github.com/Fintech-Internship-04/.github/assets/11494592/42f0ee45-c46a-4a66-9ddb-4f6a3a73930b)

![슬라이드8](https://github.com/Fintech-Internship-04/.github/assets/11494592/a94fa2fc-954b-483e-b9b0-26f9496c6edc)
![슬라이드10](https://github.com/Fintech-Internship-04/.github/assets/11494592/27f1b3e4-6bb8-4bdb-9c00-02589feba69b)


위와 같이 모임 결제에서 더치페이를 선호하는 사람들이 많음을 확인할 수 있습니다.  


![슬라이드11](https://github.com/Fintech-Internship-04/.github/assets/11494592/6d8970f7-e5b7-4dd6-821f-f7f11065ca89)


이들은 위와 같이 정산과정에서 불편함을 호소하고 있습니다.  


![슬라이드16](https://github.com/Fintech-Internship-04/.github/assets/11494592/e08d2d96-c07b-4af8-8663-456c6e5bf652)


정산을 하기 위해선 계산기 어플을 키고 일일이 계산해야 하는 번거로움이 있습니다.  


![슬라이드26](https://github.com/Fintech-Internship-04/.github/assets/11494592/bed94cc4-895f-4220-afc3-5767b5fb589f)


그 번거로움을 해결하는 서비스가 바로 저희 어?벌써? 입니다. 30초 안에 모든 모임 정산을 자동으로 완료하는 서비스입니다.  

### 🌞 타겟층

1) 술자리 등과 같은 모임 자리에서 자동 정산을 빠르게 하고자 하는 20대에서 30대 청년
2) 모임별 자동 정산 내역을 빠르게 확인하고자 하는 사람

따라서 이 서비스는 모임에서 더치페이를 많이 하는 사람들에게 적합한 서비스입니다.


### ✏️ 주요 서비스

![슬라이드27](https://github.com/Fintech-Internship-04/.github/assets/11494592/b960f872-24f2-48b2-8f1f-7387548aa971)

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

유저, 모임, 계좌 관련 기능을 구현하기 위한 DB를 설계하였습니다.

### ✏️ 화면 설계

![슬라이드41](https://github.com/Fintech-Internship-04/.github/assets/11494592/c79cef06-8fd4-412a-ac14-48455f46a68b)  

모바일 앱의 주요 화면을 Figma 툴을 활용해 디자인하였습니다.


## ⏰ 개발 기간 (2022.0 ~ 2022.06.10)

기획 : 2023.06.22 ~ 2023.08.03    
개발 : 2023.08.05 ~ 2023.08.21


# 🏃 주요기능 소개

### 1️⃣ 로그인, 회원가입



### 🛠️ 기술스택

- FrontEnd   
  ![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
  ![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

- BackEnd   
  ![Springboot](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
  ![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
  Mybatis

- Cloud
  ![AWS EC2](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
- Collaboration
  ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

### ✏️ 기획 및 설계

[📌 API 명세서](https://docs.google.com/spreadsheets/d/14fNcLsGACdjf05tymfdWs0joQEAKalX1WlGWrzz5ALA/edit#gid=14029005)

[📌 Github(Frontend)](https://github.com/2022-1-Capstone-Project/face-your-pace-frontend)

[📌 Github(Backend)](https://github.com/Fintech-Internship-04/Fintech-Internship-04-BE)
