# **라벨링 작업**

## ** 1. 이미지 데이터 라벨링 **

Labeling AI은 다양한 방식을 이용한 라벨링 작업을 지원합니다. 이미지, 음성, 텍스트 등의 정형 및 비정형 데이터를 각 상황과 목적에 맞는 라벨링 방식을 선택할 수 있습니다. 단순하고 이용이 쉬운 바운딩 박스 또는 폴리곤을 이용한 라벨링부터 스켈레톤, 키포인트, 시멘틱 세그멘테이션, 매직 툴 등 더욱 고도화 된 라벨링 기능들을 사용하여 데이터 라벨링을 진행할 수 있습니다. Labeling AI에서 지원되는 라벨링 방식들의 차이와 적용 기준에 대하여 자세히 살펴보겠습니다.
<center>
<video autoplay="" style="max-width: 80%;" loop="" muted="">
<source src="https://aimakerdslab.s3.ap-northeast-2.amazonaws.com/asset/video/labelingai_tool_ko.mp4" type="video/mp4">
</video>
</center>

1) **바운딩 박스** :  네모난 박스형태로 물체의 라벨링을 잡는 방법 <br>
2) **폴리라인**  :   선형 라인을 라벨링하는 방법<br>
3) **폴리곤**  :  물체 주의를 점으로 여러 번 찍어 더 자세하게 잡는 라벨링 방법<br>
4) **매직툴** :  복잡한 형태의 객체를 간단하고 쉽게 라벨링 <br>
&nbsp;&nbsp; > **매직툴 기능** <br>
&nbsp;&nbsp;&nbsp;   1. 매직툴은 3가지 type 제공하고 객체마다 적합한 매직툴 기능을 선택하여 이용 가능 합니다. <br>
&nbsp;&nbsp;&nbsp; 2. 민감도를 조절해 얼마나 민감하게 물체를 라벨링 할 것인지를 말합니다. 민감도는 0과 1사이로 되어 있고 1로 갈수록 만들어지는           폴리건이 작게 만들어 집니다. 

## ** 2. 텍스트 데이터 라벨링  **

텍스트 수동 라벨링은 학습 데이터의 라벨을 직접 생성하는 작업입니다.  자연어 데이터인 영화 리뷰가 나열된 텍스트 데이터를 수동 라벨링 할 수 있습니다. 예를 들어, 영화 리뷰가 나열된 텍스트 데이터를 수동 라벨링 할 수 있습니다. 

Labeling AI에서는 직접 라벨링 클래스의 개수와 이름을 정해야 합니다. 예를 들어, 위의 영화 리뷰 데이터 분석 프로젝트에서 라벨 클래스를 긍정(1), 부정(0)으로 라벨링 할 수 있습니다. AI 모델은 각 텍스트 데이터를 자연어처리로 분석하여 라벨링 값인 1, 0과의 관계를 학습할 것입니다.

#### **<p style="text-align: center;"> 텍스트 데이터 라벨링 </p>**
|id     | document     |   label|
|:----------:|:-------------------:|:-------------------:|
|9976970 |아 더빙.. 진짜 짜증나네요 목소리     |   0|
|3819312  |흠...포스터보고 초딩영화줄....오버연기조차 가볍지 않구나       |  1 |
|10265843    |     너무재밓었다그래서보는것을추천한다  |     0 |
|9045019  |교도소 이야기구먼 ..솔직히 재미는 없다..평점 조정  |      0 |
|6483659 | 사이몬페그의 익살스런 연기가 돋보였던 영화!스파이더맨에서 늙어보이기만 했던 커스틴 던스트가 너무나도 이뻐보였다 |  1 |
|5403919  |막 걸음마 뗀 3세부터 초등학교 1학년생인 8살용영화.ㅋㅋㅋ...별반개도 아까움.  |    0 |
|7797314 | 원작의 긴장감을 제대로 살려내지못했다. |  0 |
|9443947  |별 반개도 아깝다 욕나온다 이응경 길용우 연기생활이몇년인지..정말 발로해도 그것보단 낫겟다 납치.감금만반복반복..이드라마는 가족도없다 연기못하는사람만모엿네     |   0 |
|7156791  |액션이 없는데도 재미 있는 몇안되는 영화 | 1 |

## ** 3. 음성 데이터 라벨링  **
 
음성 데이터의 수동 라벨링은 인공지능의 학습을 위하여 음성 데이터에 텍스트 라벨을 직접 작성하는 작업입니다. 녹음된 음성 파일을  청취하면서 텍스트로 옮겨 적는 과정을 통해 라벨링할 수 있습니다.  




<br>
<br>
<br>
