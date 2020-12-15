## 딕셔너리 (dictionary)
<br>

Key와 Value를 한 쌍으로 갖는 자료형
<br><br>

### 쌍 추가
```python
>>> a = {1:'a',2:'b'}
>>> a[3] = [1,2,3]
>>> a
{1: 'a', 2: 'b', 3: [1, 2, 3]}
```
<br>

### 삭제 : **del**
```python
>>> a = {1:'a',2:'b'}
>>> del a[1]
>>> a
{2: 'b'}
```
<br>

### 검색
```python
>>> a = {1:'a',2:'b'}
```

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

## dict comprehension
출력표현식 : {식 for 변수 in 리스트 if 조건식}
```python
>>> a = {i:1 for i in map(int, input().split())}
1 3 5 7 9
>>> a
{1: 1, 3: 1, 5: 1, 7: 1, 9: 1}
```

<br>관련 자료 : [점프투파이썬](https://wikidocs.net/16)