<div align="center">
    
# SilverLink (실버링크)
    
독거 어르신의 일상을 기록하고, 보호자와의 연결을 돕는 AI 돌봄 콜봇 서비스

어르신들의 일상 기록 단절 문제를 해결하고, 응급 상황 발생 시 보호자 및 상담사에게 즉각적인 연결을 제공하여 골든타임을 확보하는 AI 솔루션입니다.

<img width="1200" height="500" alt="" src="images/silverlink.png" />
</div>
<br>
<br>

## 목차
- [개요](#개요)
- [기획 배경](#기획-배경-why-we-built-this)
- [기대 효과](#기대-효과-what-we-aim-to-achieve)
- [주요 기능 및 서비스](#주요-기능-및-서비스)
- [기술 스택](#기술-스택tech-stack)
- [시연 영상](#시연-영상)
- [서비스 주요 플로우](#서비스-주요-플로우)
- [시스템 아키텍처](#시스템-아키텍쳐system-architecture)
- [사용자 시나리오](#사용자-시나리오user-flow)
<br><br>

## 개요
- **개발 기간:** 2025/12/12 - 2026/02/08 (약 3주)
- **팀 구성:** 6명 (Cloud, 프론트엔드, 백엔드, AI)
- **주최:** 새싹 X 솔트룩스 AICC 풀스택 과정
- **수상:** 우수 프로젝트상(대상) 수여
<img width="700" alt="" src="images/우수프로젝트상.jpg" />
<br><br><br>

## 기획 배경 (Why we built this)
현재 독거 어르신 돌봄 환경은 물리적인 거리와 돌봄 인력의 부족으로 인해 치명적인 사각지대에 놓여 있습니다. 본 프로젝트는 현장의 세 가지 핵심 페인 포인트(Pain Points)를 해결하기 위해 시작되었습니다.

**일상 기록의 단절**

매일의 식사, 복약, 수면 등 필수적인 일상 정보가 데이터화되지 않아 질병의 전조 증상이나 건강 변화 패턴을 추적하고 관리하기 어렵습니다.

**골든타임 확보의 위기** 

예기치 못한 건강 악화나 응급 상황 발생 시, 보호자나 담당 상담사에게 즉각적으로 상황이 전달되지 않아 대응이 늦어지는 위험이 존재합니다.

**사회적 고립과 우울감**

단순한 생사 확인을 넘어, 어르신의 감정을 어루만져 주고 일상을 나눌 수 있는 따뜻한 대화 상대가 턱없이 부족합니다.
<br><br><br>

## 기대 효과 (What we aim to achieve)

SilverLink는 단순한 자동 안부 전화를 넘어 기술을 통해 단절된 가족과 사회를 다시 연결하는 것을 목표로 합니다.

**정서적 고립 해소 (어르신)** 

어제 나눈 대화를 기억하고 먼저 안부를 묻는 '세상에 단 하나뿐인 전담 AI'와의 교감을 통해 독거노인의 우울감을 완화하고 활력을 제공합니다.

**데이터 기반의 연속적 돌봄 (보호자/상담사)**

통화 내용을 바탕으로 '3줄 요약, 감정 분석, 건강 태그(#두통, #식사거름 등)'가 포함된 실행형 리포트를 매일 제공하여 끊김 없는 맞춤형 건강 관리를 가능하게 합니다.

**스마트 안전망 구축 (시스템)** 

대화 중 우울감이나 건강 이상 징후가 감지될 경우, 시스템이 즉각적으로 보호자 앱에 알림을 전송하여 신속하게 골든타임을 확보할 수 있습니다.
<br><br><br>

## 주요 기능 및 서비스
**1. 스마트 예약 발신 (Smart Outbound Call)**
- **자동 안부 전화:** 시스템이 보호자가 설정해 둔 약속된 시간에 맞춰 어르신에게 먼저 전화를 겁니다.
- **안정적인 연결 대기열:** 여러 어르신에게 동시에 전화를 걸어야 하는 상황에서도, 누락이나 지연 없이 안정적으로 통화가 연결되도록 스케줄링 시스템이 작동합니다.

**2. 개인 맞춤형 실시간 대화 (Personalized Real-time Conversation)**
- **안전한 대화 환경:** 통화 중 어르신이 주민등록번호나 주소 같은 민감한 개인정보를 말씀하셔도, AI가 이를 즉시 감지하고 비식별화(가림 처리)하여 안전하게 보호합니다.
- **과거를 기억하는 교감:** "어제 병원 다녀오신 건 어떠셨어요?"처럼 이전 대화 내용을 기억하고 먼저 물어봐 주는 등, 단순한 기계가 아닌 전담 요양보호사처럼 대화합니다.
- **사람 같은 초저지연 소통:** 어르신의 말씀이 끝나기 무섭게 1.5초 이내에 즉각적으로 반응하며, 대화가 뚝뚝 끊기지 않고 자연스럽게 이어집니다.

**3. 데이터 분석 및 보호자 연동 (Analysis & Guardian Sync)**
- **통화 직후 요약 리포트:** 전화가 끊어지면 AI가 5~10분의 긴 대화를 3줄로 요약하고, 어르신의 감정 상태(우울감, 기쁨 등)와 건강 이상 징후를 분석해 보호자의 앱으로 즉시 전송합니다.
- **보호자 안심 챗봇 문의:** 보호자가 앱에서 "최근 일주일간 어머니 식사는 어떠셨어?"라고 질문하면, AI가 그동안 쌓인 통화 기록을 찾아내어 정확하고 상세하게 답변해 줍니다.
<br><br><br>

## 기술 스택(Tech Stack)
| **분류 (Category)** | **기술 스택 (Tech Stack)** | **주요 역할 (Role)** |
| :--- | :--- | :--- |
| **AI Framework** | FastAPI, LangChain, LangGraph | API 서빙 및 에이전트 대화 흐름 제어 |
| **Backend** | Spring Boot 3.4, Spring Security | 메인 비즈니스 로직 처리 및 보안/인증 |
| **LLM / SLM** | GPT-4o-mini / Qwen 2.5 0.5B | GPT(복잡한 대화 추론), Qwen(빠른 의도 분류) |
| **Database** | MySQL, Milvus, FAISS | MySQL(데이터 저장), Milvus(RAG 검색), FAISS(대화 기억) |
| **Communication** | Twilio, Saltlux Luxia, Google V2 | Twilio(실시간 전화 스트리밍), Saltlux(TTS), Google V2(STT) |
| **Infrastructure** | AWS SQS, AWS S3, Docker | SQS(메시지 큐잉), S3(파일 저장), Docker(환경 구축) |
| **Security/PII** | Microsoft Presidio | 대화 내용 중 민감한 개인정보 자동 마스킹 |

<br><br>

## 시연 영상

### [📹시연영상](https://screenapp.io/app/v/uaQPc0twLX)
<br><br>

## 서비스 주요 플로우
### 1. 어르신 등록
<img width=700 src="gifs/regist-elder.gif">

### 2. 보호자 등록
<img width=700 src="gifs/register-guardian.gif">

### 3. 상담사 배정
<img width=700 src="gifs/assignment-counselor.gif">

### 4. 개인 맞춤형 통화
<img width=700 src="gifs/callbot.gif">

### 5. 통화 분석 및 상담사 일지 작성
<img width=700 src="gifs/summary-callbot.gif">

### 6. 보호자 확인
<img width=700 src="gifs/confirmation-guardian.gif">

### 6. 응급 상황 및 알림
<img width=700 src="gifs/emergency-callbot.gif">
<br><br>

## 시스템 아키텍쳐(System Architecture)
```mermaid
%%{init: {'theme': 'default'}}%%
flowchart TD
    %% 사용자 영역
    subgraph Client ["사용자 환경"]
        Elder["👵 어르신 (일반 전화)"]
        Guardian["📱 보호자 (모바일 앱)"]
    end

    %% 통신 및 인프라 영역
    subgraph Infrastructure ["인프라 & 통신"]
        Twilio["📞 Twilio (Voice Streaming)"]
        SQS["📨 AWS SQS (Message Queue)"]
        S3["☁️ AWS S3 (Storage)"]
    end

    %% 메인 백엔드 영역
    subgraph Backend ["Backend Framework"]
        SB["💻 Spring Boot 3.4 API"]
        SEC["🛡️ Spring Security (인증/인가)"]
        SB --- SEC
    end

    %% AI 코어 영역
    subgraph AICore ["AI Framework"]
        FA["🧠 FastAPI 서버"]
        LC["🔗 LangChain & LangGraph"]
        MEM["🧠 Mem0 (장기 기억)"]
        PII["🕵️‍♂️ MS Presidio (비식별화)"]
        
        FA --- LC
        FA --- MEM
        FA --- PII
    end

    %% LLM 및 음성 모델 영역
    subgraph Models ["LLM & TTS (Hybrid)"]
        GPT["☁️ OpenAI GPT-4o-mini"]
        Qwen["🖥️ Local: Qwen 2.5 0.5B"]
        TTS["🔊 Saltlux Luxia (TTS)"]
    end

    %% 데이터베이스 영역
    subgraph Databases ["Database"]
        RDB[("💾 MySQL RDS")]
        Milvus[("📊 Milvus/Zilliz")]
        Qdrant[("⚡ Qdrant Local")]
    end

    %% 연결 로직 (데이터 흐름)
    Guardian <-->|"REST API 요청"| SB
    Elder <-->|"음성 패킷"| Twilio
    
    SB -->|"비동기 통화 스케줄링"| SQS
    SQS -->|"Python Worker 트리거"| FA
    
    Twilio <-->|"웹소켓 스트리밍"| FA
    
    FA -->|"민감정보 필터링"| PII
    FA -->|"컨텍스트 및 기억 검색"| Qdrant
    FA -->|"RAG 검색"| Milvus
    FA -->|"단순 의도 파악/빠른 응답"| Qwen
    FA -->|"복잡한 대화 추론/요약"| GPT
    FA -->|"텍스트 전달"| TTS
    TTS -->|"음성 데이터 반환"| FA
    
    FA -->|"통화 종료 후 리포트 전달"| SB
    SB -->|"최종 데이터 저장"| RDB
    FA -->|"녹음/로그 파일 저장"| S3
```
<br><br>

## 사용자 시나리오(User Flow)
```mermaid
%%{init: {
  'theme': 'base', 
  'themeVariables': {
    'actorTextColor': '#ffffff', 
    'actorLineColor': '#ffffff', 
    'actorBkg': '#2D3748', 
    'actorBorder': '#ffffff',
    'textColor': '#000000', 
    'messageTextColor': '#000000', 
    'noteTextColor': '#000000'
  }
}}%%
sequenceDiagram
    autonumber
    actor Elder as 👵 어르신 (전화)
    actor Guardian as 📱 보호자 (App)
    participant SB as 💻 Spring Boot BE
    participant SQS as 📨 AWS SQS
    participant Worker as ⚙️ Python Worker
    participant Twilio as 📞 Twilio API
    participant AI as 🧠 FastAPI (AI Core)
    participant DB as 💾 DB (MySQL / Milvus)

    rect rgb(230, 240, 255)
    Note over SB, Twilio: 1. 통화 요청 및 워커 작동
    SB->>SQS: 통화 요청 메시지 발행
    SQS-->>Worker: 메시지 수신 (비동기 처리)
    Worker->>Twilio: 아웃바운드 통화 API 호출
    Twilio->>Elder: 전화 연결
    end

    rect rgb(255, 235, 230)
    Note over Elder, AI: 2. 대화 수행 (실시간 스트리밍)
    Elder->>AI: 🗣️ 발화 (음성 패킷 수신 및 STT)
    AI->>AI: 🛡️ Presidio (개인정보 비식별화)
    AI->>AI: 🧠 Mem0 (장기/과거 기억 검색)
    AI->>AI: 🤖 GPT-4o-mini (응답 텍스트 생성)
    AI->>AI: 🔊 Luxia (TTS 음성 패킷 변환)
    AI->>Twilio: 🎵 음성 스트리밍 송출
    Twilio->>Elder: AI 음성 답변
    end

    rect rgb(230, 255, 230)
    Note over AI, DB: 3. 분석 및 저장 (통화 종료 후)
    AI->>AI: LLM 대화 요약 및 감정 분석
    AI->>SB: 최종 리포트 저장 API 호출
    SB->>DB: MySQL에 최종 리포트 저장
    end

    rect rgb(255, 250, 205)
    Note over Guardian, DB: 4. 보호자 챗봇 문의
    Guardian->>SB: 챗봇 문의 (Proxy)
    SB->>AI: 문의 내용 전달 (FastAPI)
    AI->>DB: Milvus 벡터 검색 (유사 데이터 추출)
    DB-->>AI: 검색 결과 반환
    AI-->>SB: LLM 기반 답변 생성 및 반환
    SB-->>Guardian: 보호자 앱에 최종 답변 제공
    end
```
   1. 통화 요청:
       * Spring Boot BE → AWS SQS 발행.
   2. 워커 작동:
       * Python SQS Worker가 메시지 수신 → Twilio API 호출.
   3. 대화 수행:
       * 발화 감지 → Presidio(비식별화) → Mem0(기억 검색) → GPT-4o-mini(응답 생성) → Luxia(TTS 변환) → Twilio(음성
         송출).
   4. 분석 및 저장:
      * 통화 종료 후 LLM이 대화 요약 및 감정 분석 → Spring Boot API 호출하여 MySQL에 최종 리포트 저장.
   5. 챗봇 문의:
      * 보호자 앱 → Spring Boot(Proxy) → FastAPI Chatbot → Milvus 검색 및 답변 생성.
