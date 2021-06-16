## Time complexity in Python

### List 자료형과 기본 메소드

| Operation | Example | Big-O | Notes |
|---|---|---|---|
| Index | list[i] | O(1) | 인덱스로 값 찾기 |
| Store | list[i] = 0 | O(1) | 인덱스로 데이터 저장 |
| Length | len(list) | O(1) | 리스트 길이 찾기 |
| Append | list.append(i) | O(1) | 리스트 가장 뒤에 데이터 저장 |
| Pop | list.pop() | O(1) | 가장 뒤의 데이터 제거 |
| Clear | list.clear() | O(1) | 모든 데이터 제거 |
| Slice | list[a:b] | O(b-a) | 슬라이싱 되는 요소의 수에 비례 |
| Extend | list.extend(i) | O(len(i)) | 확장되는 길이에 비례 |
| Construction | list(...) | O(len(...)) | 데이터의 길이에 비례 |
| Compare | list1 == list2 | O(N) | 두 리스트가 동일한지 확인 |
| Insert | list[a:b] = ... | O(N) | 데이터 삽입 |
| Delete | del list[i] | O(N) | 데이터 삭제 |
| Containment | x in, not in | O(N) | 데이터 포함 여부 확인 |
| Copy | list.copy() | O(N) | 리스트 복제 |
| Remove | list.remove(...) | O(N) | 데이터 제거 |
| Pop(i) | list.pop(i) | O(N) | 제거 된 이후 값을 shift 함 |
| Extreme value | min(i), max(i) | O(N) | 전체 데이터를 확인 |
| Reverse | list.reverse() | O(N) | 리스트 뒤집기 |
| Iteration | for i in list | O(N) | 전체 데이터를 순회 |
| Sort | list.sort() | O(N Log N) | 파이썬 기본 정렬 |
| Multiply | k * list | O(k N) | 리스트의 갯수 곱셈 |

### Set 자료형과 기본 메소드

| Operation | Example | Big-O | Notes |
|---|---|---|---|
| Add	| set.add(5) | O(1) | 집합 요소 추가 |
| Containment	| x in/not in set | O(1)	| 포함 여부 확인 |
| Remove	| set.remove(..) | O(1)	| 데이터 제거 |
| Discard	| set.discard(..) | O(1) | 특정 데이터 제거 |
| Pop	| set.pop() | O(1) | 랜덤하게 하나 pop |
| Clear	| set.clear() | O(1) | similar to s = set() |
| Construction	| set(...) | O(len(...)) | 데이터 길이에 비례 |
| Compare	| set != t | O(len(s)) | 전체 데이터 동일 여부 확인 |
| <=/<	| set <= t | O(len(s)) | 부분집합 여부 |
| >=/>	| set >= t | O(len(t)) | 부분집합 여부 |
| Union	| set, t | O(len(s)+len(t)) | 합집합 |
| Intersection	| set & t | O(len(s)+len(t)) | 교집합 |
| Difference	| set - t | O(len(s)+len(t)) | 차집합 |
| Symmetric	| Diff	s ^ t | O(len(s)+len(t)) | 여집합 |
| Iteration	| for i in set: | O(N) | 전체 데이터 순회 |
| Copy	| s.copy() | O(N) | 복제 |

### Dictionary 자료형과 기본 메소드

| Operation | Example | Big-O | Notes |
|---|---|---|---|
| Store	| d[k] = v | O(1) | 데이터 저장 |
| Length | len(d) | O(1) | 길이 출력 |
| Delete| del d[k] | O(1) | 데이터 제거 |
| Get/Set |	d.get(k) | O(1) | key에 따른 value 확인 |
| Pop(i) | d.pop(k) | O(1) | pop |
| Pop item | d.popitem() | O(1) | 랜덤하게 선택해서 pop |
| Clear | d.clear() | O(1) | similar to s = {} or = dict() |
| View | d.keys() | O(1) | same for d.values() / 키값 전체 확인 |
| Construction | dict(...) | O(len(...)) | (key, value) 튜플 개수만큼 |
| Iteration | for i in dict: | O(N) | 전체 데이터 순회 |

### Summary: 자료형에 따른 시간 복잡도 비교
* 삽입, 제거, 탐색, 확인 등에서는 Set나 Dictionary가 효과적이며, 순서와 index에 따른 접근이라면 List도 괜찮다.
