## 집합 자료형 (set)
<br>

* 중복 허용 x
* 순서 x. 어떤 값이 먼저 나올지 알 수 없다.
<br>-> 인덱싱 불가. 리스트 or 튜플로 변환해야 한다.
<br><br>

### 관련 함수
* 값 1개 추가 : add
```python
>>> s1 = set([1,2,4])
>>> s1.add(3)
>>> s1
{1, 2, 3, 4}
```

* 값 여러 개 추가 : update
```python
>>> s1 = set([1,2,5])
>>> s1.update([3,4,5])
>>> s1
{1, 2, 3, 4, 5}
```
<br>

* 값 제거 : remove, discard<br>
  
  remove : 해당되는 값이 없을 경우 KeyError 발생 <br>
  discard : 해당되는 값이 없어도 에러가 발생하지 않는다.

```python
>>> s1 = {1,2,3}
>>> s1.remove(2)
>>> s1
{1,3}
>>> s1.remove(2)
Traceback (most recent call last):
  File "<pyshell#6>", line 1, in <module>
    s1.remove(2)
KeyError: 2
```

```python
>>> s1 = {1,2,3}
>>> s1.discard(2)
>>> s1
{1,3}
>>> s1.discard(2)
>>> s1
{1,3}
```
<br>

### **집합**
<br>
조건

```python
>>> a = set([1,2,3,4,5])
>>> b = set([3,4,5,6,7])
```
<br>

* 교집합
```python
>>> a & b
set([3, 4, 5])

>>> a.intersection(b)
set([3, 4, 5])
```
<br>

* 차집합
```python
>>> a-b
set([1, 2])

>>> a.difference(b)
set([1, 2])
```
* 합집합
```python
>>> a | b
set([1, 2, 3, 4, 5, 6, 7])

>>> a.union(b)
set([1, 2, 3, 4, 5, 6, 7])
```
<br>관련 자료 : [점프투파이썬](https://wikidocs.net/1015) / [파이썬 - 기본을 갈고 닦자!](https://wikidocs.net/16044)