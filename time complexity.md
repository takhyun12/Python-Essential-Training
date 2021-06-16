## Time complexity in Python

### List
* MS 엑셀의 함수 MID와 유사하게 동작하며, 문자열을 검사하여 boolean으로 return

```python
test_string = 'M-string-1002-A'

test_string.startwith('M-') # True
test_string.endwith('-C') # False

test_string.startwith('1002', 9, 13) # True
test_string.startwith('1000', 9, 13) # False
```

