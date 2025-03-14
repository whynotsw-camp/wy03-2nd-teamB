# 프로젝트 기획서

## 1. 프로젝트 정의
- **목표**: 목표: IPTV 콘텐츠 큐레이션 AI기반 구독형 개인화 숏폼 제작 서비스
- **주요 기능**:
  - IPTV에서 제공하는 공영미디어(뉴스, 다큐멘터리, 예능 등)의 콘텐츠를 AI 기반으로 분석하여 사용자 맞춤형 숏폼으로 자동 생성
  - 개인화된 추천, 자동 요약 및 하이라이트 생성

## 2. 주요 내용
- **프로젝트 기간**: 2025-03-10~ 2025-05-23
- **참여 인원**: 김진서, 이지예, 유병민, 장성권, 최동욱
- **데이터 사용처**:  AI Hub, 문화 빅데이터 플랫폼, LIFELOG

## 3. 일정 계획

| 작업 항목                  | 시작 날짜   | 종료 날짜   | 기간(일) |
|---------------------------|------------|------------|---------|
| 프로젝트 정의 및 계획 수립  | 2025-03-10 | 2025-03-12 | 3       |
| 자료 조사 및 벤치마킹       | 2025-03-12 | 2025-03-14 | 3       |
| 아이디어 도출 및 시나리오 작성 | 2025-03-17 | 2025-03-21 | 7       |
| 요구사항 도출 및 WBS 작성   | 2025-03-24 | 2025-03-28 | 7       |
| Prototype 개발 및 검토     | 2025-04-01 | 2025-05-20 | 31       |
| 최종 검토 및 발표 준비     | 2025-05-21 | 2025-05-23 | 2       |
| 프로젝트 발표              | 2025-05-24 | 2025-05-24 | 1       |

-----------------------------

# 작업 분할 구조 (WBS)

## 단계별 작업 내용
1. **기획 단계**
    - 요구사항 수집 및 분석
    - 프로젝트 범위 정의
    - 주요 기능 도출 및 우선순위 설정
2. **개발 단계**
    - 데이터 수집 모듈 개발
    - AI 분석 모듈 구현
    - 자동 편집 모듈 구축
    - 추천 엔진 모듈 개발
    - 사용자 피드백 수집 모듈 구현
3. **테스트 단계**
    - 기능 테스트
    - 성능 테스트
    - 통합 테스트
    - 사용자 피드백 반영
4. **배포 및 유지보수 단계**
    - 시스템 배포
    - 모니터링 및 로그 분석
    - 오류 수정 및 기능 개선
    - 사용자 피드백 지속 반영
### 시각 자료
![image.png](attachment:3630afff-b2ff-40eb-850c-5ed643b145fe:image.png)

---------------------------

# 요구사항 정의서

## 1. 기능 요구사항

- AI 기반 숏폼 자동 생성: 전체 IPTV 콘텐츠를 분석하여 중요 장면을 추출하고, 자동 편집
- 맞춤형 숏폼 추천: 사용자별 시청 패턴을 분석하여 최적의 숏폼 콘텐츠 제공
- 주요 키워드/장면 자동인식: AI가 영상 및 오디오 분석을 통해 핵심 장면을 자동 식별 (예: 인물 중심, 주요 대사)
- 음성-텍스트 변환(NLP): 자막 자동 생성 및 주요 발언 기반 영상 요약

## 2. 비기능 요구사항

- **성능**: 숏폼 생성 속도는 1초 이하로 지연 없어야 함
- **안정성**: 스트리밍 도중 끊김 현상 최소화
- **보안성**: 사용자 개인정보 보호를 위한 암호화 적용
- **확장성**: 다양한 미디어 포맷을 지원하여 플랫폼 확장 가능

---------------------------

# 프로젝트 설계서

## 1. 데이터 아키텍처
- **설계 개요**:
  - 데이터 수집: Open API, Open Dataset, Crawling
  - 데이터 저장: PostgreSQL, AWS S3 (Cloud Storage)
  - 분석 및 시각화: Tableau, Power BI, Python 라이브러리, D3.js

## 2. 기술 스택
**Frontend**

- HTML, CSS, JAVASCRIPT

**Backend**

- Python (Django)

**DATABASE**

- PostgreSQL

**Cloud & DevOps**

- AWS EC2 (Cloud Computing Instance)
- AWS S3 (Cloud Storage)
- AWS CloudFront (CDN)
- AWS CloudWatch Logs (Log Management)
- Nginx (Web Server)
- Gunicorn (WSGI)
- Let's Encrypt (SSL Certificate)
- Git (Version Control)
- Docker

**AI/ML**

- Pytorch
- Google Tran

## 3. 설계 이미지
![K-042.png](attachment:c75f6e64-2d27-4728-96d3-94dfd57c2ebe:K-042.png)

---------------------------

# 데이터 연동 정의서

## 1. 데이터 정의
- 목표: IPTV 콘텐츠 큐레이션 AI기반 구독형 개인화 숏폼 제작 서비스에 필요한 주요 데이터 소스를 연동하여 AI 분석 및 추천 시스템을 지원

- 데이터 소스: IPTV 플랫폼에서 제공되는 방송 데이터 및 VOD 정보
- 주요 컬럼:
  - CONTENT_ID: 콘텐츠 식별자
  - CONTENT_TYPE: 콘텐츠 유형 (예: VOD)
  - TITLE: 콘텐츠 제목
  - GENRE: 장르 (예: 뉴스, 예능, 다큐멘터리)
  - BROADCAST_DATE: 방송 일자
  - DURATION: 콘텐츠 길이
  - KEYWORDS: 주요 키워드 (자동 인식)
  - AUDIO_TEXT: 자막 및 음성 텍스트 (NLP 분석용)
  - VIEW_COUNT: 조회수
  - RATING: 콘텐츠 평점
  - USER_INTERACTIONS: 사용자의 상호작용 정보 (예: 좋아요, 댓글)

- 데이터 소스2: 사용자 정보(시청 패턴 및 피드백)
- 주요 컬럼:
  - USER_ID: 사용자 식별자
  - PROFILE_NAME: 사용자 프로필 이름
  - AGE: 연령대
  - GENDER: 성별
  - WATCH_HISTORY: 시청 기록 (콘텐츠 ID 및 시청 시간)
  - PREFERRED_GENRES: 선호 장르
  - INTERACTIONS: 사용자 상호작용 (예: 좋아요, 댓글, 시청 완료 여부)
  - FEEDBACK: 사용자 피드백 (예: 별점, 피드백 내용)
 
- 데이터 소스3: AI 분석 데이터 (영상 분석 및 키워드 추출)
- 주요 컬럼:
  - CONTENT_ID: 콘텐츠 식별자
  - KEY_SCENES: 주요 장면 (AI 분석 결과)
  - KEYWORDS: 자동 추출된 키워드
  - CHARACTERS: 등장 인물
  - TRANSCRIPT: 텍스트 변환된 대사
  - AUDIO_EMBEDDINGS: 음성 분석 결과 (텍스트 변환 및 중요 발언)

## 2. 연동 방식
- 연동 방식: API 또는 Batch 수집
  - **API 연동**: 실시간으로 사용자 상호작용 데이터 및 콘텐츠 정보를 수집하여 AI 분석 및 추천 시스템에 반영
  - **Batch 연동**: 주기적으로 IPTV 콘텐츠 및 방송 데이터를 수집하고, 분석 후 숏폼 콘텐츠 생성
- 연동 주기:  IPTV 콘텐츠 및 방송 데이터는 매일 자정에 수집하여 분석

--------------------------

# 시각화 리포트

## 1. 분석 결과 요약


## 2. 대시보드
![image.png](attachment:84555e9b-b6f1-4062-a180-7047d9e9aa55:image.png)

![image.png](attachment:71dcc144-a87a-4036-9e9a-fbd0d0ee93b6:image.png)

## 3. 제안
- 데이터를 기반으로 [구체적인 제안 내용]

--------------------------
