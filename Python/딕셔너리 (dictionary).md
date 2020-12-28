## 딕셔너리 (dictionary)
<br>

Key와 Value를 한 쌍으로 갖는 자료형
<br><br>
예시
```python
a = {1:'a', 2:'b'}
```
<br>

### 쌍 추가
```python
>>> a[3] = [1,2,3]
>>> a
{1: 'a', 2: 'b', 3: [1, 2, 3]}
```
<br>

### 삭제 : **del**
```python
>>> del a[1]
>>> a
{2: 'b'}
```
<br>

### 검색
* Key 값으로 Value 얻기
  *  **get**
  *  []
```python
>>> a.get(1)
'a'
>>> a[2]
'b'
```

* **in**
```python
>>> 1 in a
True
```
<br>

### 관련 함수들
* **keys()** : Key값만 모아 dict_keys 객체로 리턴
  ```python
  >>> a.keys()
  dict_keys([1,2])
  ```
  <br>

* **values()** : value값만 모아 dict_values 객체로 리턴
  ```python
  >>> a.values()
  dict_values(['a', 'b'])
  ```
  <br>

* **items()** : Key와 Value의 쌍을 튜플로 묶은 뒤 dict_items 객체로 리턴
  ```python
  >>> a.items()
  dict_items([(1, 'a'), (2, 'b')])
  ```
  <br>

* **clear()** : 딕셔너리 안 모든 요소 삭제
  ```python
  >>> a.clear()
  >>> a
  {}
  ```
  <br>

## dict comprehension
출력표현식 : {식 for 변수 in 리스트 if 조건식}
```python
>>> a = {i:1 for i in map(int, input().split())}
1 3 5 7 9
>>> a
{1: 1, 3: 1, 5: 1, 7: 1, 9: 1}
```

<br>관련 자료 : [점프투파이썬](https://wikidocs.net/16)