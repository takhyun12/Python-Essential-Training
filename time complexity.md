## Time complexity in Python

### List 자료형과 기본 메소드
* MS 엑셀의 함수 MID와 유사하게 동작하며, 문자열을 검사하여 boolean으로 return

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
| Compare | list1 == list2 | O(N) | 전체 리스트가 동일한지 확인 |
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
---



