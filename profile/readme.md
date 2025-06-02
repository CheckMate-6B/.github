# ✔️ 체크메이트

#### 📌 프로젝트 소개
체크메이트는 계약서를 손쉽게 작성하고 작성한 계약서를 업로드하면 LLM을 통해 분석해주는 서비스입니다.

#### 🗓️ 수행 기간
2025.04.14 ~ 2025.05.22

-----

# 👩‍💻 개발 환경
### Frontend
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=white"/>
<img src="https://img.shields.io/badge/Typescript-3178C6?style=for-the-badge&logo=Typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=Tailwind%20CSS&logoColor=white"/> <br />

### Backend
<img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white"/>
<img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/>
<img src="https://img.shields.io/badge/ClamAV-0079C1?style=for-the-badge"/>
<img src="https://img.shields.io/badge/AES--GCM-000000?style=for-the-badge&logo=lock&logoColor=white"/> <br />

### AI
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=LangChain&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/> <br />

### Database
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Qdrant-000000?style=for-the-badge"/> <br />

### Infra/DevOps
<img src="https://img.shields.io/badge/EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS%20S3-569A31?style=for-the-badge&logo=Amazon%20S3&logoColor=white"/>
<img src="https://img.shields.io/badge/CloudFront-232F3E?style=for-the-badge&logo=Amazon%20CloudFront&logoColor=white"/>
<img src="https://img.shields.io/badge/GitLab%20Runner-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white"/> <br />

### Tools
<img src="https://img.shields.io/badge/Mattermost-0058CC?style=for-the-badge&logo=mattermost&logoColor=white"/>
<img src="https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white"/> <br />

-----

# 📋 기능 요약

- **계약서 템플릿으로 계약서 작성**: 업무 유형별 사전 검증된 표준 템플릿으로 필수 항목만 입력하면 완성된 계약서 생성
- **계약서 바이러스 검사**: 계약서를 업로드 하면 ClamAV를 통해 바이러스 검사
- **계약서 분석**: 계약서를 AI를 이용해 요약, 위험조항, 누락조항, 개선사항을 생성
- **계약 질문리스트 생성**: 계약서 기준으로 AI를 통해 계약하기 전 질문리스트 생성
- **전자서명을 통한 전자문서 인증**: API를 통해 전자서명 인증 
- **실시간 알림**: 전자서명 완료, 분석완료, 질문리스트 생성이 완료 시 알림

-----

# 🔧 설계

### 시스템 아키텍처
![image](https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98.jpg)

<br/>

### ERD
![erd](https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/ERD.jpg)

-----

# 🎯 주요 화면 및 기능 소개

#### 메인화면

| 메인화면 | 뉴스 (모바일) |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%A9%94%EC%9D%B8%ED%8E%98%EC%9D%B4%EC%A7%80.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EA%B4%80%EB%A0%A8%20%EB%89%B4%EC%8A%A4.gif" width="300" /> |

#### 계약서 분석

| 업로드 | 업로드 (모바일) |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%B6%84%EC%84%9D%20%EC%97%85%EB%A1%9C%EB%93%9C.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EB%B6%84%EC%84%9D%20%ED%8C%8C%EC%9D%BC%20%EC%97%85%EB%A1%9C%EB%93%9C.gif" width="300" /> |

| 분석 결과 | 실시간 알림 및 분석 결과 (모바일) |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%B6%84%EC%84%9D%ED%8E%98%EC%9D%B4%EC%A7%80.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EB%B6%84%EC%84%9D%EA%B2%B0%EA%B3%BC%20%EB%8C%80%EC%8B%9C%EB%B3%B4%EB%93%9C.gif" width="300" /> |

#### 계약서 작성 가이드

| 작성 가이드 |
| :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EC%9E%91%EC%84%B1%20%EA%B0%80%EC%9D%B4%EB%93%9C.gif" width="300" /> |

#### 계약서 작성 전 주의사항

| 작성 전 주의 사항 | 작성 전 주의사항 (모바일) |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EC%9E%91%EC%84%B1%20%EC%A0%84%20%EC%A3%BC%EC%9D%98%EC%82%AC%ED%95%AD.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EC%9E%91%EC%84%B1%20%EC%A0%84%20%EC%A3%BC%EC%9D%98%EC%82%AC%ED%95%AD.gif" width="300" /> |

#### 계약서 작성

| 계약서 작성 | 계약서 작성 (모바일) | 질문리스트 (모바일) |
| :---: | :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EA%B3%84%EC%95%BD%EC%84%9C%20%EC%9E%91%EC%84%B1.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EA%B3%84%EC%95%BD%EC%84%9C%20%EC%9E%91%EC%84%B1.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EC%A7%88%EB%AC%B8%EB%A6%AC%EC%8A%A4%ED%8A%B8.gif" width="300" />  |

#### 마이페이지

| 마이페이지 | 분석페이지 |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%A7%88%EC%9D%B4%ED%8E%98%EC%9D%B4%EC%A7%80.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%82%B4%EA%B3%84%EC%95%BD%EC%84%9C%20-%20%EB%B6%84%EC%84%9D%ED%8E%98%EC%9D%B4%EC%A7%80.gif" width="300" /> |

| 법원 | 법원 (모바일) |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%B2%95%EC%9B%90.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EC%A3%BC%EB%B3%80%20%EB%B2%95%EC%9B%90.gif" width="300" /> |

#### 계약서 저장

| 계약서 저장 | 계약서 저장 (모바일일) |
| :---: | :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EC%B5%9C%EC%A2%85%20%EA%B3%84%EC%95%BD%EC%84%9C.gif" width="300" /> | <img src="https://github.com/CheckMate-6B/.github/blob/f66c4de0b949ecae395b9573d68e9a7c3c92d542/images/%EB%AA%A8%EB%B0%94%EC%9D%BC%20%EC%B5%9C%EC%A2%85%20%EA%B3%84%EC%95%BD%EC%84%9C.gif" width="300" /> |

#### 전자서명
| 전자서명 |
| :---: |
| <img src="https://github.com/CheckMate-6B/.github/blob/72b9d9eca3e47be16c6352f196c6a0c50563d03f/images/%EC%A0%84%EC%9E%90%EC%84%9C%EB%AA%85.gif" width="300" /> |

-----   

# 🥳 팀원
| 이영재(팀장) | 손서현 | 신승아 | 송창현 | 김성찬 | 고태연 |
| :---: | :---: | :---: | :---: | :---: | :---: |
| BE<br/>AI | BE | FE | FE | BE<br/>AI | FE<br/>DevOps |
<br/>
