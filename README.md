# Data Analysis Portfilio
----
**목차**
>
* [1. 개인 의료비 예측 프로젝트](#1-개인-의료비-예측-프로젝트)
```여러가지 회귀 모델을 사용하여 환자의 의료비에 영향을 미치는 주요 요인을 식별하고, 해당 정보를 활용하여 의료비를 예측하였습니다```
* [2. 음악 장르 분류 및 추천 프로젝트](#2-음악-장르-분류-및-추천-프로젝트)
```FCNN 딥러닝 모델로 음악 파일 별로 유사도를 확인하고 Cosine Similarity를 통하여 해당 음악과 가장 유사한 상위 5개의 음악을 추천 받는 시스템을 만들었습니다.```  
* [3. 그림 스타일 변환 프로젝트](#3-그림-스타일-변환-프로젝트)
```CycleGAN 딥러닝 모델을 활용하여 특정 그림의 스타일을 학습시켜 실제 사진의 스타일을 변환하는 모델을 생성하였습니다 ```

## 1. 개인 의료비 예측 프로젝트

* 문제정의  
```
· 환자의 의료비에 영향을 미치는 주요 요인을 식별하고, 생활 패턴 개선에 기여하기 위해 프로젝트를 진행
```  
* 프로젝트 진행  
```
· 과도한 이상치 제거로 인한 과적합과 데이터 왜곡을 방지하기 위해 IQR등의 이상치 제거의 기준을 조정
· 의료비를 기준으로 3개의 구간으로 나누어 각각 구간에 맞는 모델을 적용하여 오차를 줄이고 성능 개선
· 주요 특성(나이, bmi, 흡연 유무)을 기준으로 모델 선택 후 예측 진행
```
* 기대효과와 배운점
```
[기대효과]
· 의료비 예측 모델을 활용하여 보험 가입자들의 프로필을 개선
. 예방적 건강 서비스를 제공함으로써 보험 청구 비용을 감소시키는 방안을 모색
```
[배운점]
```
· 이상치 탐지와 데이터 전처리, 하이퍼 파라미터 튜닝 등을 통한 모델 최적화
. 의료 데이터를 다루며 의료 분야의 도메인 지식들과 의료 비용의 결정에 영향을 끼치는 주요 요인 확인
```

※ 프로젝트 링크 > [바로가기](https://github.com/HextonGit/Portfolio/tree/main/개인%20의료비%20예측%20프로젝트)  
 

## 2. 음악 장르 분류 및 추천 프로젝트

* 문제정의  
```
· 음악 스트리밍 서비스의 음악 선호도를 고려한 정확하고 개인화된 추천이 부족하다고 느껴 프로젝트 계획
· 같은 아티스트의 음악을 추천하는 것이 아닌 음악 파일 별로 유사도를 확인, 추천하는 시스템을 만드는 것이 목표
```  
* 수행역할  
```
· Logistic Regression, RandomForest, DecisionTree, XGBoost 등의 머신러닝 모델을 사용, 가장 높은 성능 확인
· CNN, FCNN 딥러닝 모델링을 통하여 훈련 및 검증과 모델 선택
· 음악 파일에서 추출한 특성들을 기반으로 Cosine Similarity를 활용하여 음악 파일 간의 유사성을 측정
. 해당 음악과 가장 유사한 상위 5개의 음악을 추천
```  
* 기대효과와 배운점
```
[기대효과]
· 기존의 비슷한 아티스트의 음악을 추천해주는 시스템보다 더욱 정확하고 개인화된 추천 시스템을 제공할 것으로 기대
[배운점]
· FCNN 이외에도 CNN과 GoogleNet등의 새로운 딥러닝 모델들을 적용하는 경험을 쌓음
· 음악 파일을 다룰 때 필요한 도메인 지식과 20 여가지의 음악적 특성에 대한 이해를 얻음
```
<br>

※ 프로젝트 링크 > [바로가기](https://github.com/HextonGit/Portfolio/tree/main/음악%20장르%20분류%20및%20추천%20프로젝트)  

## 3. 그림 스타일 변환 프로젝트

* 문제정의  
```
· 최근 생겨난 그림, 사진 생성 AI들의 저작권 관련 문제를 인식하고 이러한 생성형 AI GAN이 어떻게 작동하는지 직접 알아보기 위하여 프로젝트 계획
· 특정 스타일의 그림을 학습시킨 후 새로운 이미지의 스타일을 학습시킨 스타일로 변환하는 것이 목표
```  
* 수행역할  
```
· 각 이미지 파일에 대한 TFRecord 파일 생성과 같은 데이터 전처리
· 전이 학습, CycleGAN, VGG19 를 활용하여 모델 훈련 및 성능 확인 후 모델 선택
· CycleGAN 딥러닝 모델을 활용하여 실제 사진 이미지를 모네의 화풍으로 변환 및 새로운 이미지를 생성
```  
* 기대효과와 배운점
```
[기대효과]
· GAN 모델이 여러 그림 스타일을 학습하면, 사용자는 다양한 스타일로 이미지를 쉽게 변환할 수 있음
. 예술, 디자인 등의 분야에 도움이 되는 하나의 툴이 될 수 있을 것으로 기대
[배운점]
· CycleGAN 이외에도 VGG19와 전이 학습과 같은 이미지 관련 모델들을 적용하는 경험을 쌓음
· 이미지 파일에 처리에 대한 도메인 지식 및 통일해야 하는 이미지 파일의 종류, 크기, 특성에 대한 이해
```

※ 프로젝트 링크 - [바로가기](https://github.com/HextonGit/Portfolio/tree/main/그림%20스타일%20변환%20프로젝트)

