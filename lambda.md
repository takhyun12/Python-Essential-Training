## Lambda / Anonymous Function

* Lambda 함수는 코드를 간결하게 만들어주며, return 등의 키워드를 사용하지 않아 아주 약간의 메모리절약이 가능하다.
* 하지만 가장 큰 강점은 코드를 직관적으로 만들어준다는 점이다.

### Syntax:

```python
lambda arguments: expression

add = lambda x,y:x+y
print(add(10, 20))
```

### Usage:

* Python style과 Lambda Style의 비교

```python
def double(x):
  return x*2
```

```python
num = lambda x: x*2
print(num(10))
```

* List 정렬에서의 활용방법

```python
target = ['cat', 'tiger', 'dog', 'snake']
print(sorted(target, key=lambda x: len(x.strip())))
```
