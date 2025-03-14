# 프로젝트 기획서

## Demo
![DASHBOARD](https://github.com/user-attachments/assets/050f4433-b356-4520-873a-83c881c3058c)
![DASHBOARD2](https://github.com/user-attachments/assets/a1752474-0e2c-4c60-8fd4-212e0ed8cdad)

## 1. 프로젝트 정의
- **목표**: IPTV 콘텐츠 큐레이션 AI기반 구독형 개인화 숏폼 제작 서비스
  - **서비스 확장**: 기존 IPTV에서 제공하는 영화, 드라마, 예능, 스포츠 등과 숏폼 콘텐츠를 결합하여 새로운 서비스를 제공
  - **숏폼 콘텐츠**: 15초에서 3분 내외의 짧은 영상으로, 최근 모바일 중심의 소비에서 IPTV 등 대형 스크린으로 확장되고 있음
  - **차별화 전략**: IPTV에서 구독형 숏폼 서비스를 제공하여 기존 VOD(영화, 드라마)와 뉴스 중심의 IPTV 서비스와 차별화하고, 유튜브, 틱톡, 인스타그램 릴스와 같은 플랫폼과 경쟁력 있는 포지션을 구축

- **차별화 전략**
  | IPTV 구독형 숏폼 서비스 | 기존 유튜브/틱톡과의 차별점 |
  | --- | --- |
  | **IPTV 맞춤형 콘텐츠 제공** | 유튜브는 범용적 콘텐츠, IPTV는 전문 콘텐츠 |
  | **고품질 & 프리미엄 콘텐츠 제공** | 무료 UGC 기반이 아닌, 방송사 제작 콘텐츠 활용 |
  | **광고 기반 + 구독 모델 가능** | 유튜브는 주로 광고 기반, IPTV는 구독형 추가 가능 |
  | **IPTV 추천 엔진 활용** | IPTV의 기존 AI 추천 시스템과 연계 가능 |
    
- **기대효과**
  | 항목 | 기대 효과 |
  | --- | --- |
  | **📈 가입자 증가** | 숏폼 콘텐츠 도입으로 Z세대 & MZ세대 IPTV 유입 확대 |
  | **⏳ 체류 시간 증가** | VOD+숏폼 조합으로 IPTV 사용 시간 증가 |
  | **💰 광고 수익 증대** | 광고 삽입형 숏폼 콘텐츠 제공으로 광고 매출 증가 |
  | **📊 사용자 분석 강화** | 숏폼 시청 패턴 분석하여 맞춤형 추천 제공 |
  | **📺 IPTV 경쟁력 향상** | 유튜브, 틱톡과 차별화된 IPTV 숏폼 서비스 구축 |

- **서비스 흐름**
![FLOW](https://github.com/user-attachments/assets/e864d944-868f-4055-a916-cdd47243d62e)
  - **콘텐츠 수집**: VOD 및 방송 데이터 수집
  - **AI 분석**: 영상, 오디오, 텍스트 분석을 통해 주요 장면 및 키워드 추출
  - **숏폼 비디오 제작**: AI가 주요 장면을 편집하여 숏폼 콘텐츠 생성
  - **사용자 데이터 수집**: 사용자 시청 기록, 선호도, 피드백 수집
  - **개인화 엔진**: 사용자 맞춤형 숏폼 콘텐츠 추천
  - **사용자 피드백**: 사용자 상호작용 및 평가를 통한 지속적인 개선

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
![WBS](https://github.com/user-attachments/assets/9d721e43-ff51-448a-b394-430775a931ce)

---------------------------

# 요구사항 정의서

## 1. 기능 요구사항

| 기능 설명 | 우선순위 | 상세 내용 |
| --- | --- | --- |
| AI 기반 숏폼 자동 생성 | 필수 | 전체 IPTV 콘텐츠를 분석하여 중요 장면을 추출하고, 자동 편집 |
| 맞춤형 숏폼 추천 | 필수 | 사용자별 시청 패턴을 분석하여 최적의 숏폼 콘텐츠 제공 |
| 주요 키워드/장면 자동 인식 | 필수 | AI가 영상 및 오디오 분석을 통해 핵심 장면을 자동 식별 |
| 음성-텍스트 변환(NLP) | 중간 | 자막 자동 생성 및 주요 발언 기반 영상 요약 |

### 세부 기능 요구사항

| **기능군** | **세부 기술** | **기술 스택** | **성능 지표** |
| --- | --- | --- | --- |
| **영상 분석** | 장면 전환 감지 | OpenCV + YOLOv8 | 정확도 92%↑ |
| **콘텐츠 추출** | 핵심 프레임 스코어링 | Transformer 모델 | 처리 속도 30fps |
| **자동 편집** | 클립 스티칭 & 전환 효과 | FFmpeg + Nvidia CUDA | 렌더링 지연 <1초 |
| **맥락 이해** | 주제 기반 클러스터링 | BERT + CLIP | 토픽 일치도 88% |
| **개인화** | 사용자 반응 예측 | Apache Kafka + PyTorch | CTR 18%↑ |

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
![K-042](https://github.com/user-attachments/assets/f8817353-688c-4a89-a807-4c5db5f615f7)

---------------------------

# 데이터 연동 정의서

## 1. 데이터 정의
![데이터 정의](https://github.com/user-attachments/assets/3381d3ca-6bce-45f6-9f5a-bebc6fff02fd)

## 2. 연동 방식
- 연동 방식: API 또는 Batch 수집
  - **API 연동**: 실시간으로 사용자 상호작용 데이터 및 콘텐츠 정보를 수집하여 AI 분석 및 추천 시스템에 반영
  - **Batch 연동**: 주기적으로 IPTV 콘텐츠 및 방송 데이터를 수집하고, 분석 후 숏폼 콘텐츠 생성
- 연동 주기:  IPTV 콘텐츠 및 방송 데이터는 매일 자정에 수집하여 분석

--------------------------
