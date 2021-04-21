```python
import itertools
```

## 순열
순열 : 반복 가능한 객체 중 r개를 뽑아 나열하는 것

permutations(iterable, r)<br>
r : 몇 개의 아이템을 조합할 지 결정.  default : 전체 길이

```python
a = [1,2,3]
p = itertools.permutations(a,2)
print(list(p))
[(1, 2), (1, 3), (2, 1), (2, 3), (3, 1), (3, 2)]
```
<br>

## 조합
조합 : 반복 가능한 객체에 대해 순서와 상관 없이 r개를 뽑아 나열하는 것
combinations(iterable, r)<br>
r : 몇 개의 아이템을 조합할 지 결정. 작성하지 않을 경우 오류

```python
>>> a = [1,2,3]
>>> c = itertools.combinations(a,2)
>>> print(list(c))
[(1, 2), (1, 3), (2, 3)]
```