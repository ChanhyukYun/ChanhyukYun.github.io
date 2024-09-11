---
title:  "Privacy-preserving camera localization via paired-point lifting (2022.06 - 2023.11)"
---
  
Developing core algorithms for 3D reconstruction and camera localization that can address user's privacy concerns.
  
<br/>

### Problems in previous works
* Privacy threat is possible in 3D point cloud by reconstructing 2D images using a CNN-based model ([Pittaluga et al., CVPR 2019]())
  + Concern server-side privacy issues
  + Several approaches are given to avoid above issue, but not practical  
    1. 3D Point cloud -> 3D Line Cloud, ([Speciale et al., CVPR 2019]())  
       - Replace points with randomly directed lines, so that the CNN-based model cannot work  
       - This approach was refuted by [Chelani et al., CVPR 2021](), which shows line clouds with uniform-distributed line directions can be restored into point cloud  
      
    2. 3D Point cloud -> Save separately for each point's coordinates (e.g., x, y, z), ([Geppert et al., CVPR 2022]())
<br/>

### Methodology

### Publications  
  
#### Paper  
* Chunghwan Lee, Jaihoon Kim, **Chanhyuk Yun** and Je Hyeong Hong. "Paired-Point Lifting for Enhanced Privacy-Preserving Visual Localization.", *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition.* 2023  
  + [CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/html/Lee_Paired-Point_Lifting_for_Enhanced_Privacy-Preserving_Visual_Localization_CVPR_2023_paper.html)  
  + [GitHub](https://github.com/Fusroda-h/ppl)
  
<br/>
  
#### Patents  
* South Korea, Submitted, 10-2023-0008666, "선군 맵 데이터를 이용하는 위치 추정 방법 및 장치, 선군 맵 데이터 생성 방법"  
* US, Submitted, 18/417,235, "Localization Method and Apparatus Using Line Cloud Map Data, Line Cloud Map Data Generation Method"  

<br/>

### Organization  
[HY-Vision Lab](https://sites.google.com/view/hyvision/home?authuser=0), [Hanyang University](https://hanyang.ac.kr/)

