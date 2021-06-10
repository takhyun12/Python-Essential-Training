## zip
* zip will take two iterables and will create a tuple with each matching element in each one

```python
list1 = ['a','b','c']
list2 = [1, 2, 3]

zip(list1, list2) # return iterable object

list(zip(list1, list2)) # use list type
dict(zip(list1, list2)) # use dict type
```

* Return index method
```python
[ i2 for i1, i2 in zip(list1, list2) if i1 =='b' ] # output : 2
```
