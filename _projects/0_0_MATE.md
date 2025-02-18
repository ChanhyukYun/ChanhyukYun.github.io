---
title:  "AI Smart Meeting Assistant for Team Efficiency (MATE) (2024.12 - 2025.02)"
---

회의 중 내용 요약, 피로 탐지 및 독성표현을 탐지 해주는 AI 스마트 회의 어시스턴트 개발

<br/>

## 개발 동기
- 코로나가 창궐한 2020년 이후 온라인 화상 회의 시장 규모는 점진적으로 증가함  
- 기존 온라인 회의 서비스는 실시간 요약 기능이나 회의록 저장 기능 등이 기본적으로 지원되지 않음  
- 강남역 근처에서 93명에 대하여 설문조사 결과, 온라인 회의는 다음 문제가 있음  
  1. 오프라인 회의 대비 집중하기 어려움  
  2. 참가자 간 소통이 어려움  
  3. 회의 내용 정리가 어려움  
- 또한 온라인 회의 내용 정리는 대부분 직접 회의록을 필기하거나 문서 작성해서 이뤄지며 이에 불만이 많아, 회의 내용 자동 요약이 필요하다는 응답이 많았음  
- 요약 기능 외에도 회의록 작성이나 공유 자료 요약 기능, 그리고 독성 발언 탐지 기능 또한 필요함  

<br/>

## 참여 인원

| 이름   | 주 업무 | Link |
|--------|---------|------|
| 이예림 | PL      |  <a href="https://github.com/lyrWinterCat"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/>    |
| 안지홍 | FE      |  <a href="https://github.com/dnwn129"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/>    |
| 이승은 | SE      |  <a href="https://github.com/Greeense"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/>    |
| 고수현 | DB      |  <a href="https://github.com/csj8566"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/>    |
| 윤찬혁 | AI      |  <a href="https://github.com/ChanhyukYun"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/> |
| 박언용 | BE      |  <a href="https://github.com/onionpark"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/>    |

<br/>

## 적용된 AI 기술

|   |          **AI 기술**         | **세부 내용**                                                        |
|---|:----------------------------:|----------------------------------------------------------------------|
| 1 | Faster-Whisper<br/>(Pre-trained) | - Speech-to-Text (STT) <br/>- API 기반 Whisper 대비 약 3배 빠른 추론 속도 |
| 2 |      GPT-4o<br/>(OpenAI API)     | - 텍스트 요약 <br/>- 이미지 요약                                          |
| 3 |    KoELECTRA<br/> (Fine-tuned)    | - 회의 음성 텍스트 중 독성 표현 (욕설, 비윤리적 발언) 탐지           |
| 4 |     Pyannote<br/> (Fine-tuned)    | - 회의 중 발화자 식별                                                |
| 5 |      YOLO11<br/> (Fine-tuned)     | - 회의 참여자 얼굴 기반 피로 탐지                                    |

<br/>

## 기대효과

#### 다양한 회의 피드백
- 좋은 성과를 낸 아이디어 제공자 식별 및 포상 가능  
- 회의 중 독성 발언 감시로 건전한 회의 분위기 조성 가능  

#### 업무 효율성 향상
- 회의 중 또는 이후 요약 기능 제공으로 원활한 회의 진행 및 복기 가능  
- 주제별 요약 및 ToDo List 제공으로 불필요한 논의 최소화  

#### 회의 스트레스 감소
- 집중도 저하 시 피로 탐지 기반의 적절한 휴식 권고로 밀도 있는 회의 진행 가능  
- 회의 중 독성 발언으로 인한 감정적 스트레스 감소가 기대됨  

<br/>

## 기여도
- 독성 표현 탐지 및 얼굴 기반 피로 탐지에 사용할 AI 모델 및 공공데이터 조사  
- 얼굴 기반 피로 탐지 데이터 및 라벨링 수집 프로그램 제작  
- 독성 표현 탐지 및 얼굴 기반 피로 탐지 모델 학습  
- GPT-4o 기반 프롬프트 엔지니어링  
- STT 이후 문장 데이터 후처리 코드 제작  
- 유튜브 영상 기반 음성 데이터 크롤링을 활용한 테스트 데이터 수집  
- GPT-4o 기반 요약 프롬프트 성능 평가 기준 제작  

<br/>

## 배운 점
- 공공데이터 포털 (AI Hub)를 활용한 공공데이터 수집 방법  
- 유튜브 영상 및 음성 데이터 크롤링 방법  
- BERT 및 KoELECTRA 학습과 학습 과정 중 발생하는 문제점 해결  
- Ultralytics 기반 YOLO11 학습을 위한 데이터 라벨링 방법  
- GPT 기반 서비스에서 발생할 수 있는 할루시네이션 문제와 이를 최소화하기 위한 프롬프트 엔지니어링  

## 차후에 해볼 것들
- GPT 기반 서비스에서 발생하는 할루시네이션 억제 기법 ()  
- 문장 단위가 아닌 문단 단위의 독성표현 탐지 ()