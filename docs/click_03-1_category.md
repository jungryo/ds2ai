<link rel="stylesheet" href="./index.css">

# **카테고리 분류 모델 이용하기**

## **카테고리 분류모델이란?**

카테고리 분류 모델은 먼저 레이블 된 학습 데이터로 학습한 후, 새로 입력된 데이터가 어느 클래스에 속하는 지를 예측하는 모델입니다. 분류는 대상이 입력 데이터와 함께 제공되는지도 학습 범주에 속합니다. 신용 승인, 의료 진단, 타겟 마케팅 등과 같은 많은 영역에서 분류에 많은 응용 프로그램이 있습니다.

두 가지 이상의 데이터를 결합하여 카테고리를 분류하는 방법은 [데이터 결합](./ds2_clean_data/)에서 자세한 내용을 확인하실 수 있습니다.


### **직접 사용해보기**

### **학습 목표 : 고객 항공 이용 데이터를 활용하여 만족도 예측하기**

## **1. 데이터 확인하기**


![이미지이름](./image_clickai/data.png)<br>
[flight_service.csv]<br>
데이터 특징은 고객 성별, 고객 타입, 나 등의  기본적인 개인정보부터 시작하여 항공 만족도에 영향을 주는 요소인 여행 목적, 여행 시간, 항공내 서비스 등의 데이터까지 총 21가지의 특징과 결과인 항공 이용의 만족도 결과로 구성되었습니다.

결과인 예금결과는 'neutral or dissatisfied'와 'satisfied'로 구분됩니다.


## **2. AI 모델 만들기**

### **1) 데이터 업로드하기**

<center>
![이미지이름](./image_clickai/1.png){: width="600px",hight="300px" }<br>
데이터 업로드를 위해 DS2 DATASET을  클릭합니다.
</center> 

<center>
![이미지이름](./image_clickai/2.png){: width="600px",hight="300px" }<br>
인공지능 개발을 위한 데이터 추가를 위해 데이터 추가하기를 클릭합니다.
</center> 

<center>
![이미지이름](./image_clickai/3.png){: width="600px",hight="300px" }<br>
다운 받은 데이터는 .csv파일이기 때문에 CSV를 클릭하고 다음을 누릅니다.
</center>

<center>
![이미지이름](./image_clickai/4.png){: width="600px",hight="300px" }<br>
파일찾기 버튼을 클릭하여 다운받을 데이터를 클릭하여 업로드 합니다. 
</center> 

<center>
![이미지이름](./image_clickai/6.png){: width="600px",hight="300px" }<br>
업로드된 파일을 확인할 수 있으며 데이터 설정에 결과값 컬럽을 선택해 주세요. 
</center> 

<center>
![이미지이름](./image_clickai/7.png){: width="600px",hight="300px" }<br>
데이터가 업로드 중입니다.
</center> 

### **2) 인공지능 개발하기**

<center>
![이미지이름](./image_clickai/8.png){: width="600px",hight="300px" }<br>
해당 프로젝트에 맞는 학습형태, 선호하는 방식을 선택해 주세요.<br>
 1. 학습형태는 '정형 데이터 카테고리 분류 (Classification)' 를 선택합니다. <br>
 2. 선호하는 방식은 2가지로 나뉘어져 있으며, '정확도가 높게' 방식을 선택하겠습니다.<br>
 3. 분석/예측하고 싶은 값에 'satisfication - flight_service.csv'를 클릭합니다.<br>
</center> 

<center>
![이미지이름](./image_clickai/9.png){: width="600px",hight="300px" }<br>
데이터를 클릭하시면 사용하신 CSV파일의 데이터를 확인하실 수 있습니다.
</center> 

<center>
![이미지이름](./image_clickai/10.png){: width="600px",hight="300px" }<br>
하단을 보면 데이터 요약과 더불어 학습데이터 사용여부를 선택할 수 있습니다. <br> (분석/예측하고 싶은 값은 자동으로 사용여부가 해제됩니다.)
</center>

<center>
![이미지이름](./image_clickai/11.png){: width="600px",hight="300px" }<br>
데이터 전처리를 선택하여 전처리 하기를 원하는 값을 선택하여 전처리 할 수 있습니다.<br>
전처리 필요 시 전처리하기 버튼을 클릭하여 전처리를 실행합니다.전처리에 대한 자세한 설명은 [데이터 전처리](./ds2_clean_data.md)에서 확인하실 수 있습니다.
</center> 

<center>
![이미지이름](./image_clickai/12.png){: width="600px",hight="300px" }<br>
원하는 전처리 기능들을 선택하고 완료를 클릭합니다.
</center>

<center>
![이미지이름](./image_clickai/13.png){: width="600px",hight="300px" }<br>
완료된 전처리는 완료 표시를 통해 확인할 수 있습니다.
</center> 

<center>
![이미지이름](./image_clickai/14.png){: width="600px",hight="300px" }<br>
모든 작업이 완료 된 후, 오른쪽 상단의  Start을 클릭하여 인공지능을 생성합니다.
</center> 

<center>
![이미지이름](./image_clickai/15.png){: width="600px",hight="300px" }<br>
인공지능을 생성 중입니다.
</center> 

<center>
![이미지이름](./image_clickai/16.png){: width="600px",hight="300px" }<br>
생성 완료된 인공지능 프로젝트는 AutoML에서 확인할 수 있습니다.
</center> 

<center>
![이미지이름](./image_clickai/17.png){: width="600px",hight="300px" }<br>
인공지능 진행상태를 확인 할 수있습니다.
</center> 

## **3. 인공지능 상세보기/예측하기**

<center>
![이미지이름](./image_clickai/18.png){: width="600px",hight="300px" }<br>
CLICK AI 는 여러개의 인공지능 모델을 생성하고 모델별 상세내용을 확인하여 최적의 인공지능 모델을 선택할 수 있습니다. 모든 인공지능 모델 생성이 완료되면 모델별 예측 정확도를 확인 및 비교할 수 있고, 각 모델에 대한 상세보기, 개별예측, 일괄예측이 가능합니다
</center> 

### **1) 상세보기**

**1-1) 모델 성능 평가** 

<center>
![이미지이름](./image_clickai/19.png){: width="600px",hight="300px" }<br>
Detail 은 모델의 정확도(Accuracy)와 오차율(Error Rate)을 확인할 수 있습니다.
</center> 

**1-2) Feature importance**  

<center>
![이미지이름](./image_clickai/20.png){: width="300px",hight="600px" }<br>
Feature Importance 는 변수의 중요도로써, 각 변수가 예측값에 얼마나 큰 영향을 미치는지 나타냅니다.
</center> 

**1-3) API**

<center>
![이미지이름](./image_clickai/21.png){: width="600px",hight="300px" }<br>
API는 해당 모델을 프로그래밍 언어로 활용할 수 있도록 API 를 제공합니다. CLICK AI 의 API는 JavaScript, Python, Wget, Java 언어를 지원합니다
</center> 

**1-4) 서비스앱 이용하기**

<center>
![이미지이름](./image_clickai/22.png){: width="600px",hight="300px" }<br>
"TRAINING MODEL (모델번호)" 우측에 "서비스 앱 공유하기" 버튼을 클릭하면, [DS2.AI](http://ds2.AI) 외부에서도 예측과 분석할 수 있습니다. </center> 

### **2) 개별예측**

<center>
![이미지이름](./image_clickai/23.png){: width="600px",hight="300px" }<br>
개별예측을 선택하면, 각 변수의 값을 입력하여 하나의 예측값을 결과로 얻을 수 있습니다. 단일 예측이나 모델의 정확도를 테스트하기 위한 용도로 활용할 수 있습니다. 키에 맞는 데이터를 입력하여 결과값을 확인할 수 있습니다.
</center> 

### **3) 일괄예측**

<center>
![이미지이름](./image_clickai/24.png){: width="600px",hight="300px" } <br>
일괄예측을 선택하면, 한꺼번에 많은 데이터를 예측할 수 있습니다. '예측용 템플릿 다운로드하기'를 클릭하여 템플릿을 다운받습니다.
</center>

<center>
![이미지이름](./image_clickai/25.png){: width="600px",hight="300px" } <br>
다운받은 템플릿에 데이터를 채워 넣습니다.
</center> 

<center>
![이미지이름](./image_clickai/26.png){: width="600px",hight="300px" } <br>
데이터를 채워넣은 예측용 템플릿을 업로드하고, 다음을 클릭합니다.
</center>

<center>
![이미지이름](./image_clickai/27.png){: width="600px",hight="300px" } <br>
일괄예측이 시작되며, 알림을 통해서 일괄예측 결과를 받아 볼 수있습니다.
</center> 

## **4. 인공지능 활용하기**

<center>
![이미지이름](./image_clickai/a-18.png){: width="600px",hight="300px" }<br>
생성된 각 인공지능 모델에 대해 분석하기, 다운로드, 디플로이, 판매하기 형태로 활용이 가능합니다.
</center> 

### **1) 분석하기**

<center>
![이미지이름](./image_clickai/29.png){: width="600px",hight="300px" }<br>
분석하기를 클릭하면 각 속성 값이 결과값에 어떤 영향을 주었는지 그래프로 시각화하여 확인할 수 있습니다.
</center>

### **2) 다운로드**

<center>
![이미지이름](./image_clickai/30.png){: width="600px",hight="300px" }<br>
다운로드를 클릭하면 모델 사용권을 구매할 수 있습니다.  모델 사용권 구매시 딥러닝 모델 파일과 주피터에서 추론 기능을 사용할 수 있는 코드를 함께 이메일로 전송합니다.<br> 
\* Jetson Nano 2GB Developer Kit 의 칩셋을 별구 구매하시면 운영서버 접속없이 임베디드 제품을 통해 인공지능 모델을 활용할 수 있습니다.
</center>

### **3) 디플로이**

<center>
![이미지이름](./image_clickai/31.png){: width="600px",hight="300px" }<br>
디플로이를 선택하시면, 클라우드 서버를 임대하여 해당 모델을 베포, 운영, 관리할 수 있는 통합 MLOPS를 제공합니다.
</center>

<center>
![이미지이름](./image_clickai/32.png){: width="600px",hight="300px" }<br>
원하는 클라우드 제공사와 지역을 선택하시면 사용가능한 INSTANCE 목록을 확인할 수 있습니다.<br>
\* google 클라우드, azure의 사용을 원하시면 별도의 문의가 필요합니다. 
</center>

<center>
![이미지이름](./image_clickai/33.png){: width="600px",hight="300px" }<br>
원하는 INSTANCE 선택 후 하단의 "CREATE CLUSTER"를 클릭하시면, [스카이허브 배포하기](.\ds2_waytodeploy.md)를 통해 연동된 MLOPS를 활용할 수 있습니다.
</center>

### **4) 판매하기**

<center>
![이미지이름](./image_clickai/34.png){: width="500px",hight="200px" }<br>
판매하기를 선택하면 생성한 모델을 [DS2.AI](http://ds2.AI) 의 AI Market 에 판매할 수 있습니다. 해당 모델의 희망가격과 판매 옵션을 선택하여 판매요청을 클릭해주세요. AI 모델 적정성 검토 및 데이터 보안 절차를 거쳐 AI Market에 업로드 됩니다.
</center>

<center>
![이미지이름](./image_clickai/35.png){: width="600px",hight="300px" }<br>
판매 가능 판정한 모델은 AI Market의 상품리스트에서 확인할 수 있으며, 고객의 모델이 필요한 다른 사용자가 구매하면 직접 책정한 금액의 수익이 발생합니다.(20% 수수료 발생)
</center>
<br>
<br>
<br>
<br>
<br>
