### 4. Digit Recognizer Analysis
> #### 주제
  0~9까지의 숫자가 적힌 손글씨가 나타내는 실제 숫자 예측
> #### 모델 유형
  Classification Model
  
> #### 데이터 설명 
1. Target value : 'label' Feature들이 나타내는 숫자의 실제 값
1. Features : 0~9까지의 숫자들의 손글씨 이미지, 784(28*28) pixels로 구성되어 있고 각 값들은 음영에 따라 0에서 255사이의 값을 가진다.
		   
> #### 주요 내용 
1. Image Data Preprocessing(one-hot-encoder, EDA(Exploratory data analysis))
1. CNN(Convolutional Neural Network)에 적용하기 위한 Weights, Bias 설정
1. CNN모델 layer설정(Hidden layers, helper function 등)

> #### 참고 링크
1. https://www.kaggle.com/kakauandme/digit-recognizer/tensorflow-deep-nn
