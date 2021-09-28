# Pytorch Essential Training note

* references : https://teamsparta.notion.site/Pytorch-1-7669d355f573451cbf5ebfeb74c584e7#3f0f21ddd7544decaa01385c0dfb90fb

## 딥 러닝을 위한 기초수학

### 직선의 방적식(함수) `f(x)=ax+b`

* 일차함수는 a는 기울기, b는 y절편(y축과 만나는 점)으로 구성된다
* a의 값과 그리고 b의 값에 따라서 직선의 위치는 달라집니다.

### ML에서의 방정식(가설) `H(x)=wx+b`

* 딥러닝에서는 w는 가중치(weight), b는 편항(bias)로 구성된다
* w의 값과 b의 값에 따라서 직선의 위치는 달라진다

![w1](https://user-images.githubusercontent.com/41291493/134908731-b68ae42b-343c-48dc-93af-e63e5441f729.png)

### 시그마는 누계를 의미하므로 나눗셈을 추가하여 딥러닝에서는 평균을 수식으로 표현한다

### 접선(tangent line)

* 접선은 어떤 곡선을 한 점에서 만나며 그 점에서 곡선과 같은 방향, 즉 같은 기울기를 가지는 직선을 의미함

![tangent line](https://user-images.githubusercontent.com/41291493/134908691-67509715-a7d1-4317-a357-16aecb8266b6.png)

 ### 스칼라(Scalar)
 
* 스칼라(Scalar)는 하나의 상수를 의미합니다. `var1 = torch.tensor([1])`

* add, sub, mul, div `torch.add(var1, var2)`

###  벡터(Vector)

* 벡터(Vector)는 상수가 두 개 이상 나열된 자료구조이다. `vector1 = torch.tensor([1, 2, 3])`

* N 차원 벡터라고 부른다면 여기서 N은 벡터 안에 숫자가 몇 개있는지를 의미합니다.

* 내적 연산(dot product) `torch.dot(vector1, vector2)`

* a1 x b1 + a2 x b2 + a3 x b3를 우리는 벡터의 내적이라고 합니다.

### 행렬(Matrix)

* 행렬(Matrix)는 2개 이상의 벡터 값을 가지고 만들어진 값으로 행과 열의 개념을 가진 숫자의 나열입니다.

* `matrix1 = torch.tensor([[1, 2], [3, 4]])`

* 행렬의 곱셈 `torch.matmul(matrix1, matrix2)`

![tensor](https://user-images.githubusercontent.com/41291493/135062903-0186068f-6035-46ab-a6d9-9eebe1dd6d38.png)

