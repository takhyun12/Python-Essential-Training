## Numpy
### 행렬의 곱셈
* numpy를 사용하면 행렬의 곱셈 등을 훨씬 빠르고 쉽게 사용할 수 있음

```python
import numpy as np
def solution(A, B):
    return (np.matrix(A) * np.matrix(B)).tolist()
```

* 알고리즘을 통한 두 행렬의 곱셈

```python
def solution(arr1, arr2):
    answer = [[0 for _ in range(len(arr2[0]))] for _ in range(len(arr1))]
    for i in range(len(arr1)):
        for j in range(len(arr2[0])):
            for k in range(len(arr1[0])):
                answer[i][j] += (arr1[i][k] * arr2[k][j])
    return answer
```

* pythonic한 두 행렬의 곱셈

```python
def productMatrix(A, B):
    return [[sum(a*b for a, b in zip(A_row,B_col)) for B_col in zip(*B)] for A_row in A]
```
