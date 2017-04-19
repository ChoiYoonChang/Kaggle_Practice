# Kaggle_Practice
- 이 Repository는 kaggle kernel의 연구를 위한 repository입니다.
- 순서는 프로젝트가 진행된 순서로 기재되어 있습니다. 
- 세부 내용은 각 프로젝트 노트북에서 확인 할 수 있습니다. 

## 각 프로젝트 내용 설명
### Titanic_Machine Learning from Disaster
- 분석 주제 : 타이타닉호 탑승자들의 생존여부 예측
- 예측 모델 유형 : Classification
- Data 설명 
1. Target value : 'Survived(생존여부)', 0: 사망 / 1: 생존
1. Features : 타이타닉 탑승자들의 고객 정보(성별, 나이, 지불 운임 금액 등)
		   
- 주요 내용 
1. Feature Engineering : 각 column별 분석(데이터 합치기, 나누기 등) 
1. 예측 모델 적용(Logistic Regression, SVM, Random Forests, KNN)

--------------------------------------------------------------

### House Prices
- 분석 주제 : 집과 관련된 여러 정보를 활용하여 집의 'Sale Prices' 예측
- 예측 모델 유형 : Regression
- Data 설명 
1. Target value : 'SalePrices' 를 예측 하는 것이다. continuous numeric variable 이다.
1. Features : 집과 관련되어있는 여러 Features(위치, 지역, 집크기, 인접 도로와의 거리, 난방 유형 등) 80개
		   
- 주요 내용 
1. Feature Engineering : Skewd Data를 log를 취해줌으로서 정규화 해준다.
1. Regularization : L1, L2 둘다 적용하여 RMSE를 계산하다 / L2(Lasso)를 이용해서 Feature Selection을 해본다.
1. Keras에 모델을 적용한다. 
--------------------------------------------------------------


### QUORA Question Pairs Analysis
- 분석 주제 : 질문 사이트 QUORA에 올라온 질문들의 중복 여부를 판단해보자.
- 예측 모델 유형 : Classification
- Data 설명 
1. Target value : 'Is_duplicate' 질문의 중복 여부를 나타냄(0: 중복 X / 1: 중복 O)
1. Features : Raw text의 형태의 QUORA 질문들, 각 질문마다 부여된 id값
		   
- 주요 내용 
1. NLP(자연어 처리) 분석 : Character, Word 기준에 따른 텍스트 분석, TF-IDF
1. Training set과 Test set의 target value rate 불균형을 해소하기 위한 Data Rebalancing
1. XGBoost 모델 적용
--------------------------------------------------------------


### Digit Recognizer Analysis
- 분석 주제 : 0~9까지의 숫자가 적힌 손글씨가 나타내는 실제 숫자 예측
- 예측 모델 유형 : Classification
- Data 설명 
1. Target value : 'label' Feature들이 나타내는 숫자의 실제 값
1. Features : 0~9까지의 숫자들의 손글씨 이미지, 784(28*28) pixels로 구성되어 있고 각 값들은 음영에 따라 0에서 255사이의 값을 가진다.
		   
- 주요 내용 
1. Image Data Preprocessing(one-hot-encoder, EDA(Exploratory data analysis))
1. CNN(Convolutional Neural Network)에 적용하기 위한 Weights, Bias 설정
1. CNN모델 layer설정(Hidden layers, helper function 등)
--------------------------------------------------------------


### Two sigma Financial Modeling
- 분석 주제 : 익명화된 데이터를 가지고 target value를 가장 잘 나타내는 예측 모델 만들기
- 예측 모델 유형 : Regression
- Data 설명 
1. Target value : 익명화된 'y'값
1. Features : 시간 흐름에 따라 변화하는 값을 가진 익명화된 금융 상품들
		   
- 주요 내용 
1. Feature Engineering(상관계수 계산, EDA(Exploratory data analysis))
1. 높은 상관계수 값을 가지는 Feature들의 scatter, 누적 분포 살펴보기
--------------------------------------------------------------



	
