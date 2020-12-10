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
>>> 1 in a
True
```

<br>관련 자료 : [점프투파이썬](https://wikidocs.net/16)