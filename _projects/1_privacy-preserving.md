---
title:  "Paired-Point Lifting for Enhanced Privacy-Preserving Visual Localization (2022.06 - 2023.02)"
---
  
Developing core algorithms for 3D reconstruction and camera localization that can address user's privacy concerns.
  
<br/>

## 연구 동기
* Privacy threat is possible in 3D point cloud by reconstructing 2D images using a CNN-based model ([Pittaluga et al., CVPR 2019]())
  + Concern server-side privacy issues
  + Several approaches are given to avoid above issue, but not practical  
    1. 3D Point cloud -> 3D Line Cloud, ([Speciale et al., CVPR 2019]())  
       - Replace points with randomly directed lines, so that the CNN-based model cannot work  
       - This approach was refuted by [Chelani et al., CVPR 2021](), which shows line clouds with uniform-distributed line directions can be restored into point cloud  
      
    2. 3D Point cloud -> Save separately for each point's coordinates (e.g., x, y, z), ([Geppert et al., CVPR 2022]())
<br/>

## 참여 인원
- 이정환 (한양대학교 융합전자공학과)  
- 김재훈 (Samsung Electronics, KAIST)  
- 윤찬혁 (한양대학교 융합전자공학과)  
- 홍제형 (한양대학교 융합전자공학과)  
<br/>

## 방법


<br/>

## 기여도
#### InvSfM 모델 PyTorch로 이식
- 기존 tensorflow v1로 개발 및 배포된 InvSfM (Pittaluga et al., CVPR 2019) 모델을 PyTorch로 재구현하고 배포된 가중치를 이식  
- 향후 연구 확장성 및 다양한 실험을 용이롭게 하기 위함  

#### 영상 역복원의 정량 및 정성적 평가
- Cambridge Landmakrs, Energy Landscape 데이터셋에 대한 영상 역복원 후 정량 및 정성적 평가  
- 제안하는 방법에 알맞은 시나리오 (50% 확률로 점이 swap, 점 위치 오차)에서의 영상 역복원 실험 및 평가  

#### CVPR 2023 논문, supplementary 및 특허 자료 작성 참여  
- Overleaf를 활용한 논문, supplementary 작성 및 첨삭  
- Supplementary에 필요한 영상물 제작  

<br/>

## 배운점
- **작성중**

<br/>
## Publications  

#### Paper  
* Chunghwan Lee, Jaihoon Kim, **Chanhyuk Yun** and Je Hyeong Hong. "Paired-Point Lifting for Enhanced Privacy-Preserving Visual Localization.", *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition.* 2023  
  + [CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/html/Lee_Paired-Point_Lifting_for_Enhanced_Privacy-Preserving_Visual_Localization_CVPR_2023_paper.html)  
  + [GitHub](https://github.com/Fusroda-h/ppl)  

#### Patents  
* South Korea, Submitted, 10-2023-0008666, "선군 맵 데이터를 이용하는 위치 추정 방법 및 장치, 선군 맵 데이터 생성 방법"  
* US, Submitted, 18/417,235, "Localization Method and Apparatus Using Line Cloud Map Data, Line Cloud Map Data Generation Method"  

