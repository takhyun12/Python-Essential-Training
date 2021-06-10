## arguments unpacking
* Default arguments를 통해 method overloading을 핸들링하기 좋다

```python
class student:
  def sum(*args):
    nums = args[1:]
    sum = 0
    
    for num in nums:
      sum += num
      
    return sum
    
s1 = student()
print(s1.sum(2, 3)) # 5
print(s1.sum(1,1,1,1,1,1)) # 6
```

