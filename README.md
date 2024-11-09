<div align="center">
<img src="https://github.com/user-attachments/assets/18ecee70-eb0d-4d6b-b0cf-3b4662c358a8" width="300">
<br>
<h3>
  <a href="https://nanalmoa.site/login">
    <img src="https://img.shields.io/badge/나날모아_바로가기-FF6B6B?style=for-the-badge&logo=internetexplorer&logoColor=white" alt="나날모아"/>
  </a>
</h3>
</div>

## 📋 기획 배경

2025년, 한국 사회는 65세 이상 노인 인구가 20%를 넘는 초고령사회에 진입 예정입니다. 시니어는 점차 사회의 주요 구성원으로 자리 잡고 있으나, 빠르게 발전하는 디지털 기술에 적응하는 데 어려움을 겪으며 일상생활에서 디지털 기술로부터 소외되고 있습니다.

복약이나 일정을 관리하는 기존 서비스들이 있지만, 시니어들이 사용하기에는 제약이 많았습니다. 이에 저희는 AI 기능과 그룹 관리 기능, 관리자 기능을 중심으로 시니어 친화적인 서비스를 기획하게 되었습니다.

## ⏰ 개발 기간
- 2024.09.02 ~

## 💡 프로젝트 소개

나날모아는 시니어를 위한 손쉬운 지능형 일정관리 서비스입니다. 최소한의 동작(터치/클릭)으로 일정을 등록할 수 있도록 하는 것을 목표로 하며, PWA를 통해 다양한 플랫폼(웹, Android, iOS)에서 동일한 사용자 경험을 제공합니다.

### 프로젝트 목표
- 시니어 친화적인 UI/UX 제공
- AI 기술을 활용한 일정 등록 자동화
- 관리자-피관리자 시스템을 통한 효율적인 일정 관리
- 크로스 플랫폼 지원

## 🎯 메인 기능

### 1. 간편한 로그인/회원가입
- 전화번호 기반 자체 로그인
- 카카오, 네이버 소셜 로그인
- CoolSMS 플랫폼을 통한 전화번호 인증

### 2. AI 기반 일정 등록
- 음성 인식을 통한 일정 등록
  - Whisper ASR: 음성-텍스트 변환
  - GPT-4-mini: 일정 정보 추출
- 이미지 인식을 통한 복약 일정 등록
  - Clova OCR: 처방전 텍스트 추출
  - 자동 복약 일정 생성

### 3. 그룹 및 관리자 기능
- 가족, 친구와의 일정 공유
- 관리자의 피관리자 일정 조회/관리
- 그룹 초대 및 수락/거절

### 4. 캘린더 기능
- 자체 구현 캘린더
- 일간/월간 일정 조회
- 직관적인 일정 표시

## 🛠 기술 스택

### Frontend
<div>
<img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black">
<img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=pwa&logoColor=white">
<img src="https://img.shields.io/badge/nginx-009639?style=for-the-badge&logo=nginx&logoColor=white">
</div>

### Backend
<div>
<img src="https://img.shields.io/badge/nestjs-E0234E?style=for-the-badge&logo=nestjs&logoColor=white">
<img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white">
<img src="https://img.shields.io/badge/postgresql-4169E1?style=for-the-badge&logo=postgresql&logoColor=white">
</div>

### AI/External Services
<div>
<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white">
<img src="https://img.shields.io/badge/Naver_Clova-03C75A?style=for-the-badge&logo=naver&logoColor=white">
</div>

### Infra
<div>
<img src="https://img.shields.io/badge/amazon_ec2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white">
<img src="https://img.shields.io/badge/amazon_rds-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white">
<img src="https://img.shields.io/badge/github_actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">
<img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
</div>

## 🏗 서비스 아키텍처
![{467870D5-2DFC-4AB9-B901-A42516E44D63}](https://github.com/user-attachments/assets/6b887643-a6f5-4225-802c-fa529985d15e)

- Nginx를 통한 프록시 라우팅
  - /api 요청 → Backend
  - 그 외 요청 → Frontend
- 프론트엔드/백엔드 서버 분리 구성
- SSL 인증서를 통한 HTTPS 지원
- 이미지, 음성 데이터 처리를 위한 인스턴스 분리

## 👥 팀 소개

<div>


### AI
| <img src="https://github.com/Baguette-bbang.png" width="150"> | <img src="https://github.com/mooner92.png" width="150"> |
|:---:|:---:|
| [강영민](https://github.com/Baguette-bbang) | [최명헌](https://github.com/mooner92) |
| Baguette-bbang | mooner92 |

### Backend
| <img src="https://github.com/Baguette-bbang.png" width="150"> | <img src="https://github.com/nullisdefined.png" width="150"> |
|:---:|:---:|
| [강영민](https://github.com/Baguette-bbang) | [김재우](https://github.com/nullisdefined) |
| Baguette-bbang | nullisdefined |

### Frontend
| <img src="https://github.com/jellysoo97.png" width="150"> | <img src="https://github.com/paengjiwoo.png" width="150"> | <img src="https://github.com/chae-dahee.png" width="150"> |
|:---:|:---:|:---:|
| [박소연](https://github.com/jellysoo97) | [팽지우](https://github.com/paengjiwoo) | [채다희](https://github.com/chae-dahee) |
| jellysoo97 | paengjiwoo | chae-dahee |

</div>
