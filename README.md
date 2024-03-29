# **22.07_LotteMembers // 제7회 롯데멤버스 빅데이터 경진대회**
https://aifactory.space/competition/detail/2063
***
### **분석 과제**
 **고객 구매 데이터 기반 예측 모델 생성 및 개인화 마케팅 제안**

### **주제** : 구매 경험이 없는 상품을 추천하는 추천시스템 개발
    1. 사용자 별 구매 경험이 있는 상품들에 대하여 구매 패턴을 바탕으로 자체 선호도 산출
    2. 인공신경망 기반 추천시스템을 활용하여, 구매 경험이 없는 상품들의 선호도를 예측
    3. 예측된 선호도만을 바탕으로 개인에게 맞춤 추천 서비스를 제공하는 프로모션 제시

*** 
### 최종 결과
#### 1차 탈락
    - 자체적으로 고안한 선호도 점수 산정 방식이 논리적이지 못했음.
    - Validation을 이용해 평가한 결과, 선호도 예측 점수 성능이 만족스럽지 못했음.



***
***
### Team Project

#### Teaming   (팀장)김현, 김나형, 이승준 ***(in Dongguk_University_Stat)***


***

### **Data**
![image](https://user-images.githubusercontent.com/90736934/209744799-93b82ec4-8551-401c-993f-74991734b4b6.png)



***

### **전처리**

- 분석 목적인 상품 추천에 맞게 유통사 관련 데이터만 사용. 제휴사는 사용하지 않음

- 여러개의 유통사들에 대하여 판매되는 상품을 통해 대형마트, 백화점, 편의점 등 **예측**

- 상품 구매 횟수, 대분류 구매 횟수, 상품 구매 간격 등을 바탕으로 Custom 선호도 점수 생성

***

### **모델링**
- 각 유통사 별로 상품 추천 모델을 학습.

- 사용자 정보, 구매 이력 등을 바탕으로 **안 사본 상품**의 선호도를 추정한 후, 그 중에서 상위 상품들을 추천


***



### **활용 방안**

    1. 개인화 상품 광고 - 선호도 기반 가중 Sampling 한 유통사, 상품을 추천
    2. 유통사 구독 서비스 - 고객이 선택한 유통사에 유료 구독 서비스를 제공하여, 맞춤 상품 추천 및 Lpay 혜택 제공
    3. 평균 예측 점수 상위 5개 대분류를 스탬프 목록으로 선정 -> 안사본 상품들을 예측 점수 기반으로 추천 -> 스탬프 찍기 미션

***

### ***thanks***
