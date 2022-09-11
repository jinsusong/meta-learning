# meta-learning
* metric-based
* model-based
* optimization-based
  * Deep learning model은 gradient에 대한 backpropagation을 통해서 학습한다. 하지만 이런 gradient-based optimization은 적은 수의 training sample을 다루기 위해서 만들어진 것이 아닐뿐더러, 적은 optimization step내에서 converge되지 않는다. Optimization algorithm을 수정해서 적은 수의 example만 가지고 model이 잘 학습할 수 있는 방법이 있을까? 그것이 바로 optimization-based approach가 적용된 meta-learning algorithm이 지향하는 목표


# Optimization-based 
* LSTM Meta-learner 
  * [Paper](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://openreview.net/pdf?id=rJY0-Kcll)
* First-Order MAML
  * [Paper]()
* Reptile
  * [Paper](https://arxiv.org/abs/1803.02999)


# 용어
* way : 데이터 클래스의 개수  (ex. 개고양이 분류기 - 2 way classification)
* shot, point : 데이터의 개수
* query : test data (엄연히 따지자면 validation data)
* source : train data

# Investigating Meta-Learning Algorithms for Low-Resource Natural Language Understanding Tasks
* BERT
* MT-DNN
* 학습 절차
  * 레이블이 지정되지 않은 모델 매개변수를 사전 학습 , 데이터세트
  * MAML(Model Agnostic Meta Learning), First-order MAML 또는 Reptile을 사용하여 매개변수 메타 학습 
  * 대상 작업의 매개변수 미세 조정

# Leveraging Task Transferability to Meta-learning for Clinical Section Classification with Limited Data
* First-Order-MAML
* Normalized Negative Conditional Entropy
  * 도메인 내 데이터를 미세 조정하지 않고 소스 모델과 레이블이 지정된 target 샘플만 사용
  * f를 source task로 학습 
  * f에 target sample을 주면 target sample에 예측된 source label 지정
  * Z = {x_i, ^y_i, z_i}   
  * empirical joint distribution & empirical marginal distribution
* huristic search
* back huristic search 
* meta-learning 
  * replite 초기화 , bert 학습 
  * sampling batches 
   * Dou et al (2019) 동일한 전략 사용
   
