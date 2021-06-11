## List
### Merging two arrays(List)
* Java에 비해 Python은 매우 쉽게 병합이 가능함

```java
int[] arr1 = {1,2,3};
int[] arr2 = {4,5,6};

int arr1Length = arr1.length;
int arr2Length = arr2.length;

int[] resultArray = Array.copyOf(arr1, arr1Length + arr2Length);
System.arrayCopy(arr2, 0, resultArray, arr1Length, arr2Length);  
```

```python
arr1, arr2 = [1,2,3], [4,5,6]
result = arr1 + arr2
```

