# meta-learning
* metric-based
* model-based
* optimization-based
  * Deep learning model은 gradient에 대한 backpropagation을 통해서 학습한다. 하지만 이런 gradient-based optimization은 적은 수의 training sample을 다루기 위해서 만들어진 것이 아닐뿐더러, 적은 optimization step내에서 converge되지 않는다. Optimization algorithm을 수정해서 적은 수의 example만 가지고 model이 잘 학습할 수 있는 방법이 있을까? 그것이 바로 optimization-based approach가 적용된 meta-learning algorithm이 지향하는 목표
  * First-Order-MAML
  * Normalized Negative Conditional Entropy
  * huristic search
  * back huristic search 

# Investigating Meta-Learning Algorithms for Low-Resource Natural Language Understanding Tasks
* BERT
* MT-DNN
* 학습 절차
  * 레이블이 지정되지 않은 모델 매개변수를 사전 학습 , 데이터세트
  * MAML(Model Agnostic Meta Learning), First-order MAML 또는 Reptile을 사용하여 매개변수 메타 학습 
  * 대상 작업의 매개변수 미세 조정
