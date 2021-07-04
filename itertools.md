## itertools

* Python 내장 라이브러리인 itertoolssms 특정 배열에 대하여 순열이나 조합을 효과적으로 만들 수 있다.

### Usage:

#### product()

* 중첩된 loop에 해당하는 데카르트의 곱

```python
import itertools
itertools.product('ABCD', repeat=2)

# 결과: AA AB AC AD BA BB BC BD CA CB CC CD DA DB DC DD
```

#### permutations()

* 가능한 모든 순서, 반복 X

```python
import itertools
itertools.permutations('ABCD', 2)

# 결과: AB AC AD BA BC BD CA CB CD DA DB DC
```

#### combinations()

* 정렬된 순서, 반복 X

```python
import itertools
itertools.combinations('ABCD', 2)

# 결과: AB AC AD BC BD CD
```

* 반복되지 않는 정렬된 

```python
def sample(s: str, k: int) -> int:
    words = list(itertools.combinations(s, k))
    words.sort(reverse=True)
    return "".join(words[0])
```

#### combinations_with_replacement()

* 정렬된 순서, 반복 O

```python
import itertools
itertools.combinations_with_replacement('ABCD', 2)

# 결과: AA AB AC AD BB BC BD CC CD DD
```
