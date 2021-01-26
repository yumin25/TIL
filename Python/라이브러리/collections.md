## deque
double ended queue.<br>
앞, 뒤에서 데이터를 처리할 수 있는 queue형 자료구조. 스택과 큐의 기능을 모두 가진 객체
```python
from collections import deque
a = deque([1,2,3])
```
<br>

* append() : 마지막에 원소 한 개 추가. O(1)
```python
>>> a.append(4)
>>> a
deque([1, 2, 3, 4])
```

* appendleft() : 왼쪽(앞)에 원소 한 개 추가. O(1)
```python
>>> a.appendleft(0)
>>> a
deque([0, 1, 2, 3])
```

* extend() : 마지막에 추가. O(k)
```python
>>> a.extend([2,3,4])
>>> a
deque([1, 2, 3, 4])
```

* extendleft() : 마지막에 추가. O(k)
```python
>>> a.extendleft([0,-1])
>>> a
deque([-1, 0, 1, 2, 3, 4])
```

* pop() : 마지막 항목 리턴하면서 삭제. O(1)
```python
>>> a.pop()
2
>>> a
deque([0, 1])
```

* popleft() : 왼쪽(앞) 항목 리턴하면서 삭제. O(1)
```python
>>> a.popleft()
0
>>> a
deque([1])
```

* rotate(n) : 원소를 우측으로 n만큼 이동. O(k)
```python
>>> a.rotate()
deque([3, 1, 2])
```
