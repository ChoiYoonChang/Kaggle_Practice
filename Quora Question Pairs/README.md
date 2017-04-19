## QUORA Question Pairs Analysis
> #### 주제
  질문 사이트 QUORA에 올라온 질문들의 중복 여부를 판단해보자.
> #### 예측 모델
  Classification Model
  
> #### 데이터 설명 
1. Target value : 'Is_duplicate' 질문의 중복 여부를 나타냄(0: 중복 X / 1: 중복 O)
1. Features : Raw text의 형태의 QUORA 질문들, 각 질문마다 부여된 id값
		   
> #### 주요 내용 
1. NLP(자연어 처리) 분석 : Character, Word 기준에 따른 텍스트 분석, TF-IDF
1. Training set과 Test set의 target value rate 불균형을 해소하기 위한 Data Rebalancing
1. XGBoost 모델 적용

> #### 참고 링크
1. https://www.kaggle.com/anokas/quora-question-pairs/data-analysis-xgboost-starter-0-35460-lb
1. https://www.kaggle.com/philschmidt/quora-question-pairs/quora-eda-model-selection-roc-pr-plots
