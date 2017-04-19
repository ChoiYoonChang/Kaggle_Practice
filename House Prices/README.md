## House Prices
> #### 주제
  집과 관련된 여러 정보를 활용하여 집의 'Sale Prices' 예측
  
> #### 예측 모델 유형
  Regression Model
  
> #### 데이터 설명 
1. Target value : 'SalePrices' 를 예측. 이 값은 continuous numeric variable 형태를 가지고 있다.
1. Features : 집과 관련되어있는 여러 Features(위치, 지역, 집크기, 인접 도로와의 거리, 난방 유형 등) 80개
		   
> #### 주요 내용 
1. Feature Engineering : Skewd Data를 log를 취해줌으로서 정규화 해준다.
1. Regularization : L1, L2를 적용하여 RMSE를 계산한다 / L2(Lasso)를 이용해서 Feature Selection을 실시한다.
1. Keras에 모델을 적용한다. 

> #### 참고 링크
1. https://www.kaggle.com/apapiu/house-prices-advanced-regression-techniques/regularized-linear-models
1. https://www.kaggle.com/pmarcelino/house-prices-advanced-regression-techniques/comprehensive-data-exploration-with-python
