---
title:  "Privacy-preserving camera localization via feature augmentation (2023.01 - 2024.02)"
---
  
Developing core algorithms for 3D reconstruction and camera localization that can address user's privacy concerns.
  
<br/>

## 연구 동기
- 시각적 국소화 기법은 사용자의 영상정보와 기구축한 맵 데이터를 비교하여 사용자의 위치 정보를 추론하는 방법임  
- 클라우드 기반 시각적 국소화 서비스는 사용자의 이미지 쿼리 (특징정보)가 유출될 경우 원본 영상이 복원되는 문제가 존재  
  ([Dangwal et al., BMVC 2021]())  
- 상기 문제를 해결하기 위한 기존 특징정보 은닉 방법들은 다음과 같은 문제가 있음
  1. 위치 정보 추론 성능이 떨어지거나 ([Dusmanu et al., CVPR 2021]())  
  2. 딥러닝 기반이라 수학적으로 검증되지 않으며 코드가 제공되지 않음 ([Ng et al., CVPR 2022]())
- 알고리즘 기반의 새로운 특징정보 은닉 방법을 제안하여 위치 추론 성능이 크게 떨어지지 않으면서도 영상 역복원을 저지하고자 함  

<br/>

## 참여 인원
- 윤찬혁 (한양대학교 융합전자공학과)  
- 이종우 (한양대학교 인공지능대학원)  
- 홍제형 (한양대학교 융합전자공학과, 인공지능대학원)  

<br/>

## 방법

#### 핵심 알고리즘
- **작성중**

#### 2D 쿼리 특징정보 기반 영상 역복원 모델 구현
- 코드를 제공하지 않는 영상 역복원 연구 (Dangwal et al., BMVC 2021)를 논문을 참고하여 직접 구현  
- SIFT 뿐만 아니라, HardNet 및 SOSNet의 특징정보 기반 영상 역복원 모델 학습 및 성능 평가  
- A100 x 4 또는 A6000 x 4를 distributed-data parallel (DDP) 활용하여 모델 학습

#### 알고리즘 파훼 시도를 상정한 공격 시나리오 성능 평가
-  **작성중**

<br/>

## 기여도
- 방법론 제시  
- 알고리즘 개발  
- 영상 역복원, 시각적 국소화 성능 평가  
- 논문 및 특허 작성  

## 배운점
- 작성중

## Publications  
  
#### Paper  
* **Chanhyuk Yun** and Je Hyeong Hong. "A Feature Augmentation Approach for Privacy-Preserving Image Queries.", Master's thesis, *Hanyang University*, 2023  
  + [GitHub (CVPR Submission codes)]()
  
#### Patents   
* South Korea, Submitted, 10-2024-0023612, "개인정보 유출 방지를 위한 시각적 국소화 방법 및 이를 실행하는 장치"
