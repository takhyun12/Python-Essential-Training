## zip
* zip will take two iterables and will create a tuple with each matching element in each one

```python
my_set = {1,1,1,2,'e','e',2,3,3,3,3,3,3}

my_set # output: {1,2,3,'e'}
```

* set 기반의 list 중복제거 방법

```python
def remove_duplicates(input_list):
  if len(input_list) == len(set(input_list)):
    return "No duplicates"
    
  clean_list = list(set(input_list))
  return clean_list

remove_duplicates([1,2,3,4,4,5])
```
