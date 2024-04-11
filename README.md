# INTRO
## Ⅰ. AI (Artificial Intelligence)
<img src="./a_intro/images/intro.png" width="800px">

<br/>

### 1. Rule-base AI
- 특정 상황을 이해하는 전문가가 직접 입력값(문제)과 특징을 전달(규칙)하여 출력값(정답)을 내보내는 알고리즘이다.
- 광범위한 데이터 수집, 정리 또는 교육이 필요하지 않으므로 전문가의 기존 지식을 기반으로 비지니스 규칙을 정의하여 구현 복잡성을 줄일 수 있다.
- 의사 결정 프로세스가 명시적인 "if-then" 사전 정의 규칙에 의존하므로 높은 투명성을 제공한다.
- 본질적으로 정적이며 유연성이 없기 때문에, 사전 정의된 규칙을 수동으로 조정하여 변화나 진화하는 조건에만 적응할 수 있다.
- 사전 정의된 규칙이 명확한 지침을 제공하지 않는 모호하거나 불확실한 상황에 직면할 때 어려움을 겪을 수 있다.
- 미리 정의된 기준에 의존하면, 전문가 개인의 편견이 들어갈 수 밖에 없고, 이로 인해 미묘한 행동을 설명하지 못할 수 있으며, 잠재적으로 불공평하거나 부정확한 평가로 이어질 수 있다.

<br/>
<br/>

### 2. Machine Learning AI
- 데이터를 기반으로 규칙성(패턴)을 학습하여 결과를 추론하는 알고리즘이다.
- 현실 세계의 패턴을 분석하여 개발자가 직접 코드를 작성하는 것이 어려웠으나 머신러닝을 이용해서 해결할 수 있다.

- <sub>※</sub> 데이터 마이닝, 음성 인식(언어 구분), 영상 인식(이미지 판별), 자연어 처리(번역, 문맥 찾기)에서 머신러닝이 적용된다.  
<sub>※ 데이터 마이닝이란, 대규모 데이터 안에서 체계적이고 자동적으로 통계적 규칙이나 짜임을 분석하여 가치있는 정보를 빼내는 과정이다.</sub>
- 데이터의 패턴을 학습하여 이를 통해 예측 등을 수행할 수 있다.

<br/>

#### 2-1. 지도 학습 (Supervised Learning)
입력값(문제)과 출력값(정답)을 전달하면, 알아서 특징을 직접 추출하는 방식이다.  
다른 입력값(문제)과 동일한 출력값(정답)을 전달하면 새로운 특징을 알아서 추출한다.

문제(Feature, 독립변수)와 답(Target, 종속변수, Label)을 주는 것이다.
- 분류 (이진 분류? = 코로나 양성/음성, 사기 번호/일반 번호 등 단일 값 예측) > 범주형 = 분류  
  다중분류 = 약 21개 중에 하나 먹어야함
- 회귀 (1년 뒤의 매출액, 내일 주식 가격 등 연속 값 예측) > 수치형 = 회귀

<sub>※ 사수 같은 느낌.. 문제랑 정답 AI한테 알려줌</sub>

<br/>

#### 2-2. 비지도 학습 (Unsupervised Learning)
입력값(문제)만 전달하고 정답 없이 특징만 추출하는 학습이다.
추출한 특징에 대해 AI가 출력값(정답)을 부여하여 입력값(문제)은 출력값(정답)이라는 것을 알아낸다.

문제(Feature)를 주고 답은 주지 않는 것이다.
- 군집화(클러스터링, 비슷한 문제를 분석하여 편을 나누어 각 편으로 모으는 것)
- 차원 축소 (문제이 개수를 압축(축소)하여 함축된 의미를 찾아내는 것)

<sub>※ 사수가 없는 느낌... 문제만 던져주기</sub>

<br/>

#### 2-3. 강화 학습 (Reinforcement Learning)  
https://kr.mathworks.com/discovery/reinforcement-learning.html

<br/>

#### ○ Machine Learning의 단점
- 데이터에 의존적이다 (Garbage In, Garbage Out), 데이터가 안 좋으면 결과도 안 좋을 수 밖에 없다.  
  ※ 데이터에 의존적이던 머신러닝을 해소하기 위해 나온 건 딥러닝
- 학습 데이터로 잘 만들어진 로직을 가진 모델일지라도 실제 데이터 적용 시 정확한 결과가 나오지 않을 수 있다.
- 머신러닝 학습을 통해 로직이 생기면, 나온 결과가 어떻게 이렇게 나왔는 지에 대한 분석이 쉽지 않다(블랙박스).
- 데이터를 넣으면 원하는 것처럼 좋은 결과를 얻기란 쉽지 않다.

<br/>
<br/>

### 3. R vs Python
#### 3-1. R
개발 언어에 익숙하지 않지만, 통계 분석에 능한 현업 사용자일 경우  
오랜 기간동안 쌓인 다양하고 많은 통계 패키지

<br/>

#### 3-2. Python
직관적인 문법, 객체지향 함수형 프로그래밍 언어, 다양한 라이브러리  
다양한 영역 (운영체제, 서버, 네트워크, 등)으로 연계 및 상용화하기 좋음

<br/>
<br/>

### " 머신러닝과 딥러닝은 R보다는 "파이썬"을 사용하자! "

<br/>
<br/>
<br/>
<br/>
<br/>

# classifier
## Ⅰ. classifier
### 1. 분류 (Classifier)
- 대표적인 지도학습 방법 중 하나이며, 다양한 문제와 정답을 학습한 뒤 별도의 테스트에서 정답을 예측한다.
- 주어진 문제와 정답을 먼저 학습한 뒤 새로운 문제에 대한 정답을 예측하는 방식이다.
- 이진 분류 (Binary Classification)의 경우 정답은 0(음성, Negative)과 1(양성, Positive)과 같이 True, False값을 가진다.
- 다중 분류 (Muticlass Classification)는 정답이 가질 수 있는 값은 3개 이상이다(예: 0, 1, 2, 3).

<br/>

#### 1-1. 피처 (Feature) : 독립변수
- 데이터 세트의 일반 컬럼이며, 2차원 이상의 다차원 데이터까지 통들어 피처라고 한다.
- 타겟을 제외한 나머지 속성을 의미한다.
  ※ 컬럼은 전체를 의미, 타겟을 제외한 하나는 피처라고 부름

<br/>

#### 1-2. 레이블 (Label), 클래스(Class), 타겟(Target), 결정(Decision) : 종속변수
- 지도 학습 시, 데이터의 학습을 위해 주어지는 정답을 의미한다.
- 지도 학습 중, 분류의 경우 이를 레이블 또는 클레스라고도 부른다.

<br/>

<img src="./b_classifier/images/feature_target.png" width="600ox" style="margin-left: 10px">

<br/>
<br/>

### 2. 분류 예측 프로세스
<img src="./b_classifier/images/classifier_flow.png">

<br/>

#### 2-1. 데이터 세트 분리
**tran_test_split(feature, target, test_size, random_state)**

- 학습 데이터 세트와 테스트 데이터 세트를 분리해 준다.
- feature : 전체 데이터 세트 중 feature
- target : 전체 데이터 세트 중 target
- test_size : 테스트 세트의 비율(0 ~ 1) 
- random_state : 매번 동일한 결과를 원할 때, 원하는 seed(기준점)를 작성한다.

<br/>

#### 2-2. 모델 학습
**fit(train_feature, train_target)**
- 모델을 학습시킬 때 사용한다.
- train_feature: 훈련 데이터 세트 중 feature
- train_target: 훈련 데이터 세트 중 target

<br/>

#### 2-3. 평가
**accuracy_score(y_test, predict(X_test))**
- 모델이 얼마나 잘 예측했는지를 "정확도"라는 평가 지표로 평가할 때 사용한다.
- y_test: 실제 정답
- predict(X_test): 예측한 정답

<br/>
<br/>
<br/>

## Ⅱ. decision tree
### 1. 결정 트리 (Decision Tree)
- 매우 쉽고 유연하게 적용될 수 있는 알고리즘으로서 데이터의 스케일링, 정규화 등의 데이터 전처리의 의존도가 매우 적다.
- 학습을 통해 데이터에 있는 규칙을 자동으로 찾아내서 Tree 기반의 분류 규칙을 만든다.
- 각 특성이 개별적으로 처리되어 데이터를 분할하는데 데이터 스케일의 영향을 받지 않으므로 결정트리에서는 정규화나 표준화 같은 전처리 과정이 필요없다.
- 영향을 가장 많이 미치는 feature를 찾아낼 수도 있다.
- 예측 성능을 계속해서 향상시키면 복잡한 규칙 구조를 가지기 때문에 <sub>※</sub>과적합(Overfitting)이 발생해서 예측 성능이 저하될 수도 있다.
- 가장 상위 노드를 "루트 노드"라고 하며, 나머지 분기점을 "서브  노드", 결정된 분류값 노드를 "리프 노드"라고 한다.

<br/>

<img src="./b_classifier/images/decision_tree.png"  width="550" style="margin: 20px 0 20px 20px">

<br/>

- 복잡도를 감소시키는 것이 주목적이며, 정보의 복잡도를 불순도(Impurity)라고 한다.
- 이를 수치화한 값으로 지니 계수(Gini coeficient)가 있다.
- 클래스가 섞이지 않고 분류가 잘 되었다면, 분순도가 낮다.
- 클래스가 많이 섞여 있고 분류가 잘 안 되었다면, 분순도가 높다.
- 통계적 분산 정도를 정량화하여 표현한 값이고, 0과 1사이의 값을 가진다. (0의 값을 가질 수록 과적합(Overfitting))
- 지니 계수가 낮을 수록 분류가 잘 된 것이다.

---

<sub>※ 과적합이란, 학습 데이터를 과하게 학습시켜서 실제 데이터에서는 오차가 오히려 증가하는 현상이다.</sub>

<br/>

<img src="./b_classifier/images/overfitting.png" width="350" style="margin-left: -10px">
※ 맨 처음에는 과소적합.. 에러가 많이남

<br/>
<br/>

### 2. Graphviz
- 결정트리 모델을 시각화할 수 있다.
- https://graphviz.org/download/  
  graphviz-9.0.0 (64-bit) EXE installer [sha256]
- https://drive.google.com/file/d/1oCXidIjNAvUT2UcNFEdhRfFhnZ96iHrp/view?usp=sharing

<br/>
<br/>

### 3. Feature 별 중요도
**각 feature가 분류를 나누는 데에 얼마나 큰 영향을 미쳤는지를 표기하는 척도이다.**
- feature_importances_
- 분류를 결정하는 데에 얼만큼 기여했는 지를 feature 별로 수치를 리턴해 준다.

<br/>
<br/>

### 4. 결정 트리의 과적합
- 위에서 알아낸 것처럼 petal length, petal width, 2개의 feature만으로도 분류가 가능하기 때문에, 2차원 산점도를 통해 시각화할 수 있다.
- 마지막까지 노드가 분리되었기 때문에 과적합이 발생했을 가능성이 있고, 이를 <sub>※</sub>하이퍼 파라미터 튜닝을 통해 해결할 수 있다.

<sub>※ 하이퍼 파라미터란 최적의 훈련 모델을 구현하기 위해 알고리즘의 수치를 조정할 수 있는 변수를 의미한다.</sub>

<br/>
<br/>
<br/>

## Ⅲ. 데이터 전처리
### 1. StandardScaler()
- 데이터의 평균을 0, 분산을 1이 되도록, 표준 정규분포를 따르게 하는 스케일링
- ± 1.96을 벗어나면 이상치로 판단한다.
- <code>from sklearn.preprocessing import StandardScaler</code>

<br/>
<br/>

### 2. MinMaxScaler()
- 데이터가 0~1 사이에 위치하도록 최소값은 0, 최대값은 1로 변환한다.
- 서로 다른 단위의 feature끼리 비교가 가능해진다.
- <code>from sklearn.preprocessing import MinMaxScaler</code>

<br/>
<br/>

### 3. MaxAbsScaler()
- 모든 값을 -1~1 사이에 위치하도록, 절대값의 최소값은 0, 최대값은 1이 되도록 변환한다.
- 양의 방향에 대한 단위뿐 아니라 음의 방향에 대한 단위까지 스케일링하고자 할 때 사용한다.
- <code>from sklearn.preprocessing import MaxAbsScaler</code>

<br/>
<br/>
<br/>

## Ⅳ. 교차 검증 (Cross Validation)
- 기존 방식에서는 데이터 세트에서 학습 데이터 세트와 테스트 데이터 세트를 분리한 뒤 모델 검증을 진행한다.
- 교차 검증 시, 학습 데이터를 다시 분할하여 학습 데이터와 모델 성능을 1차 평가하는 검증 데이터로 나눈다.

<br/>

<img src="./b_classifier/images/cross_validation01.png" width="500px">

<br/>

### 1. 교차 검증의 장단점
- 👍 특정 데이터 세트에 대한 과적합 방지
- 👍 데이터 세트 규모가 적을 시 과소적합 방지
- 👎 모델 훈련, 모델 평가에 소요되는 시간 증가
- 즉, 과적합을 피하고 하이퍼 파라미터를 튜닝함으로써 모델을 일반화하고 신뢰성을 증가시키기 위한 목적이다

<br/>
<br/>

### 2. 교차 검증의 종류
#### 2-1. K-Fold
- k개의 데이터 폴드 세트를 만든 뒤 k번 만큼 학습과 검증 평가를 반복하여 수행하는 방식.
- 학습 데이터와 검증 데이터를 정확히 자르기 때문에 타겟 데이터의 비중이 한 곳으로 치중될 수 있다.
- 예를 들어, 0, 1, 2 중에서 0, 1, 두 가지만 잘라서 검증하게 되면 다른 하나의 타겟 데이터를 예측할 수 없게 된다.
- Stratified K-Fold로 해결한다.

<br/>

#### 2-2. Stratified K-Fold
- k-Fold와 마찬가지로 k번 수행하지만, 학습 데이터 세트와 검증 데이터 세트가 가지는 타겟 분포도가 유사하도록 검증한다.
- 타겟 데이터의 비중을 항상 똑같게 자르기 때문에 데이터가 한 곳으로 치중되는 것을 방지한다.
<br/>

<img src="./b_classifier/images/cross_validation02.png" width="600px">

※ 평균 검증 결과가 나오게 된다.

<br/>

#### 2-3. GridSearchCV
- 교차 검증과 최적의 하이퍼 파라미터 튜닝을 한번에 할 수 있는 객체이다.
- max_depth와 min_samples_split에 1차원 정수형 list를 전달하면,  
  2차원으로 결합하여 격자(Grid)를 만들고 이 중 최적의 점을 찾아낸다.
- 딥러닝에서는 학습 속도가 머신러닝에 비해 느리고,  
  레이어(층)가 깊어질 수록 조정해 주어야 할 하이퍼 파라미터 값이 많아지기 때문에,  
  RandomSearchCV에서 대략적인 범위를 찾은 다음, GridSearchCV로 디테일을 조정하는 방식을 사용한다.

<br/>

<img src="./b_classifier/images/grid_search_cv.png" width="500px">

<br/>
<br/>

### 3. 편하게 수행할 수 있는 교차 검증
**cross_val_score(estimator, x, y, cv, scoring)**  
- estimator: classifier 종류 모델이면 내부적으로 startified K-Fold로 진행된다.
- x: features
- y: targets
- cv: 폴드 세트 개수
- scoring: 평가 함수, 정확도(accuracy) 외에 다른 것은 다른 장에서 배운다.

<br/>
<br/>

### 4. GridSearchCV
**GridSearchCV(estimator, param_grid, cv, refit, return_train_score)**
- estimator: 학습할 모델 객체 작성
- param_grid: dict 형태로 전달해야 하며, 주요 key 값은 max_depth, min_samples_split이다.
- cv: 폴드 세트 개수
- refit: 최적의 하이퍼 파라미터로 전달한 모델 객체를 다시 훈련하고자 할 때 True를 전달한다.
- retrun_train_score: 교차 검증 점수를 가져올 지에 대해 True 또는 False를 전달한다.

<br/>
<br/>
<br/>

## Ⅴ. 분류 (Classification) 성능 평가 지표
### 1. 정확도 (Accuracy)
- 직관적으로 모델 예측 성능을 나타낼 수 있다.
- 2진 분류일 경우 데이터 구성에 따라 타겟 데이터 분포가 불균형하다면, 정확도 한 가지만으로는 적합한 성능 평가 지표가 될 수 없다.
- 강아지와 고양이 모두 무조건 생존으로 예측하는 모델이 있다고 가정한다.  
  생존한 강아지 80마리와 사망한 고양이 20마리를 테스트하면, 정확도는 80%이다.
  이 모델을 사용하면, 사망한 강아지 혹은 고양이를 절대 예측할 수 없다.

<br/>

<img src="./b_classifier/images/accuracy.png" width="400px">

<br/>
<br/>

### 2. 오차 행렬 (Confusion Matrix)
- 학습된 분류 모델이 예측을 수행하면서 얼마나 예측에 오류가 있는지도 함께 보여주는 지표이다.
- 데이터가 한 곳으로 치우친 것도 확인할 수 있으며, TP, TN, FP, FN, 4가지로 구성되어 있다.
- 오차 행렬로 분류 성능 평가 지표의 모든 것을 구할 수 있다(정확도, 정밀도, 재현율, F1 Score, ROC AUC)

<br/>

<img src="./b_classifier/images/confusion_matrix01.png" width="600px">  

<br/>

1. TN: 예측한 값은 음성이고, 실제 값도 음성일 때 (맞춤)
2. FP: 예측한 값은 양성이고, 실제 값은 음성일 때 (틀림)
3. FN: 예측한 값은 음성이고, 실제 값은 양성일 때 (틀림)
4. TP: 예측한 값은 양성이고, 실제 값도 양성일 때 (맞춤)

<br/>

- 위 강아지와 고양이의 생존률 예측 모델의 오차 행렬은 다음과 같이 나온다.  
  
<br/>

<img src="./b_classifier/images/confusion_matrix02.png" width="600px">  

<br/>

- 100마리 전부 생존(음성, Negative)으로 예측했으며, 그 중 80마리는 실제 음성이고, 나머지 20마리는 실제 양성이기 때문이다.
- 보통 2진 분류일 경우 음성과 양성을 구분하는 의료학, 연구분야 등에서 많이 사용되며, 두 가지 상황으로 나눌 수 있다.

<br/>

1. 질병이나 이상이 없는데도 양성으로 오진하는 것을 방지하기 위해
  - 특이도(Specificity): 정상을 정상으로 진단하는 비율(▲TN)
  - 재현율(Recall)이 낮아지고 정밀도(Precision)가 높아질 수 있다.
2. 암 진단에서 양성인 환자를 놓치지 않고 최대한 많이 식별하기 위해
  - 민감도(Sensitivity): 질병이 있는 사람을 질병이 있다고 진단하는 비율(▲TP)
  - 재현율(Recall)이 높아지고 정밀도(Precision)가 낮아질 수 있다.

- 1.의 경우 Positive보다는 Negative 예측 정확도를 높일 것이다.  
  ▲TN, ▼TP, 또한, Positive로 예측하는 경우가 매우 작기 때문에, ▼FP
- 2.의 경우 Negative보다는 Positive 예측 정확도를 높일 것이다.  
  ▲TP, ▼TN, 또한, Negative로 예측하는 경우가 매우 작기 때문에, ▼FN
- 📌결과적으로 정확한 판단이 아님에도 불구하고 정확도가 매우 높게 나타나는, 수치적인 판단 오류를 해결해기 위해서는 특이도와 민감도를 잘 조절해야한다.  

<br/>
<br/>

### 3. 정밀도 (Precision)
- 예측을 Positive로 한 대상 중, 예측과 실제 값이 Positive로 일치한 데이터의 비율을 뜻한다.
- ▲TP, ▼FP일 경우 정밀도가 상승한다.
- precision_score()를 사용하여 정밀도를 구할 수 있다.

<br/>
<br/>

### 4. 재현율 (Recall)
- 실제 값이 Positive인 대상 중, 얼마나 놓치지 않고 Positive로 예측했는 가의 비율을 뜻한다.
- ▲TP, ▼FN일 경우 재현율이 상승한다.
- recall_score()를 사용하여 재현율을 구할 수 있다.

<br/>
<br/>

### 5. 정밀도와 재현율의 트레이드 오프 (Trade-off)
분류 시, 결정 임계값(Threshold)을 조정해서 정밀도 또는 재현율의 수치를 높일 수 있다.

<br/>

 가정: 구급대원 AI가 교통사고 현장에서 피해자를 병원으로 이송해야할지 판단해야 하는 시나리오.
- Dead (Positive): 피해자가 이미 사망했을 경우
- Alive (Negative): 피해자가 아직 살아있을 경우  

<br/>

- TP: 모델이 Dead를 Dead로 올바르게 분류한 경우
- FP: 모델이 Alive를 Dead로 잘못 분류한 경우 (error I)
- TN: 모델이 Alive를 Alive로 올바르게 분류한 경우
- FN: 모델이 Dead를 Alive로 잘못 분류한 경우 (error II)

<br/>

- error I의 비용(FP)은 error II의 비용(FN)보다 훨씬 더 나쁘다! ▼ FP, ▼ error I

<br/>

<img src="./b_classifier/images/threshold.png" width="500px">

<br/>

- 정밀도 (Precision): 모델이 Dead로 예측한 환자 중에서 실제로 Dead인 환자의 비율을 나타낸다. 즉, 양성으로 예측한 결과 중 얼마나 많은 것이 진짜 양성인지 측정한다.  
- 재현율 (Recall): 실제 Dead 피해자 중에서 모델이 Dead로 정확하게 예측한 피해자의 비율을 나타낸다. 즉, 모델이 얼마나 많은 Dead 피해자를 "놓치지 않고(재현율)" 감지했는지 측정한다.  

<br/>

- 이는 정밀도를 높여야 하며, Threshold(임계값)을 높여서 FP를 낮추고(▲정밀도), FN을 높여야 한다(▼재현율).
- 즉, Negative(Alive)로 예측할 확률이 높아져야 생명을 구할 확률이 높아지고, Threshold value(임계값)를 높여주는 것이다.
- 위의 시나리오처럼 한 쪽의 수치를 강제로 높이면 다른 한 쪽의 수치는 떨어지며,  
  이를 정밀도와 재현율의 "트레이드 오프"라고 한다.
- 임계치가 높아지면 정밀도가 높아진다. 반대로 임계치가 낮아지면 재현율이 높아진다.

<br/>
<br/>

### 6. F1 Score
- 2진 분류 모델의 성능을 평가하는 지표 중 하나이다.
- 정밀도(Precision)와 재현율(Recall)의 조화 평균(모든 데이터에 동일한 가중치)으로 계산되는 성능 측정 지표이다.
- 정확도(Accuracy)와 같이 전체 성능에 대한 지표가 아닌 타겟 데이터별 성능을 자세히 분석하는 평가지표이다.
- 정밀도(Precision)와 재현율(Recall), 두 개의평가 지표를 모두 고려하여 예측 성능을 평가하기 때문에 두 지표의 평균치를 구하는 조화 평균을 사용하여 조금 더 정확하게 모델의 예측 성능을 평가할 수 있다.
- 텍스트 분류, 정보 검색, 암 진단 등에서 사용되는 모델의 성능을 평가할 수 있다.

<br/>

<img src="./b_classifier/images/trade_off.png" width="600px">

<br/>

- F1 Score는 0~1까지 점수를 매길 수 있으며, 0에 가까울 수록 정밀도와 재현율 모두 낮다는 뜻이다.

<br/>
<br/>

### 7. ROC Curve, AUC
- ROC(Receiver Operating Characteristic)는 수신기 동작 특성이라는 뜻이고, 이러한 이름이 붙은 이유는 2차 세계대전 때 무선 기기 성능 평가 때 사용되었기 때문이다.
- FPR이 변할 때, TPR이 어떻게 변하는지를 나타내는 곡선이며, FPR이 급격히 떨어지더라도 TPR은 천천히 떨어지는 것이 좋은 성능을 가진 모델로 판단한다.

<br/>

<img src="./b_classifier/images/roc_auc.png" width="400px">

<br/>

- AUC(Area Under the Curve)는 ROC 곡선 밑의 면적을 구한 것으로써, 일반적으로 1에 가까울수록 좋은 수치이다.
- ROC Curve가 축에 붙을 수록(좌상단 모서리) 좋은 성능을 나타내는 것이며, 높이와 및변이 1인 사각형으로 가정했을 경우 ROC Curve가 축에 붙을 수록 AUC 면적이 넓어지며 1에 가까워진다.
- 모델이 양성과 음성을 얼마나 잘 분류하는지 시각화할 수 있다.
- 보통 F1 Score가 0.7 이상일 경우 좋은 모델이라고 간주한다.

<br/>

<img src="./b_classifier/images/evaluation.png" width="230px">