## 리스트 (List)

<br>관련 자료 : [docs.python](https://docs.python.org/3/tutorial/datastructures.html) / [점프투파이썬](https://wikidocs.net/14)  / [코딩 도장](https://dojang.io/mod/page/view.php?id=2281) <br>


### 관련 함수

* 리스트로 변환 : **list(변수)**
```python
>>> a = '123456'
>>> b = list(a)
>>> b
['1', '2', '3', '4', '5', '6']
```
<br>

* 요소 추가 : **append**
```python
>>> a = [1,2,3]
>>> a.append(4)
>>> a
[1, 2, 3, 4]
>>> a.append([5,6])
>>> a
[1, 2, 3, 4, [5, 6]]
```
<br>

* 요소 여러 개 추가 (확장): **extend**
```python
>>> a = [1,2,3]
>>> a.extend([4,5])
>>> a
[1, 2, 3, 4, 5]
```
<br>

* 특정 인덱스에 요소 추가 : **insert**, **슬라이싱 이용**<br>
  insert(a,b) : a번째 인덱스에 b 요소 삽입
```python
>>> a = [1,2,3]
>>> a.insert(1,4)
>>> a
[1, 4, 2, 3]
```

 슬라이싱 이용

 ```python
>>> a = [1,2,3,4,5]
>>> a[2:4]=[6,7]
>>> a
[1, 2, 6, 7, 5]
```
<br>

* 요소 수정
```python
>>> a = [1,2,3]
>>> a[2] = 4
>>> a
[1, 2, 4]
```
<br>

---
<br>

* 요소 삭제 : **del, remove** <br>
    del : 지정 인덱스 값 삭제 <br>
    remove : 첫번째로 나오는 값 삭제
```python
>>> a = [1,2,3]
>>> del a[0]
>>> a
[2, 3]
```
```python
>>> a = [1,2,3,2]
>>> a.remove(2)
>>> a
[1, 3, 2]
```
<br>

* 요소 끄집어내기 : **pop**<br>
  pop() : 맨 마지막 값 리턴 후 삭제<br>
  pop(x) : x번째 리턴 후 삭제

```python
>>> a = [1,2,3]
>>> a.pop()
3
>>> a
[1, 2]
```
```python
>>> a = [1,2,3]
>>> a.pop(1)
2
>>> a
[1, 3]
```
<br>

---
<br>

* 길이 구하기 : **len(변수)**
```python
>>> a = [1,2,3]
>>> len(a)
3
```

* 최솟값 구하기 : **min(변수)**
```python
>>> a = [1,2,3]
>>> min(a)
1
```

* 최댓값 구하기 : **max(변수)**
```python
>>> a = [1,2,3]
>>> max(a)
3
```
<br>

---
<br>

* 정렬<br>
  - **리스트 변수.sort()**
  - **sorted**(리스트 변수, 정렬 기준이 되는 key, reverse=True)<br><br>

  sort()와 sorted의 차이점 : sort는 원본 리스트의 값을 직접 수정하고 sorted는 원본의 값은 그대로이며 새로운 정렬된 리스트를 반환한다.<br>
  
  reverse = True 를 사용할 시 내림차순으로 정렬된다.

  시간 복잡도 : O(nlogn)

```python
a = [2,1,3]

>>> a.sort()
>>> a
[1,2,3]

>> sorted(a)
[1,2,3]
>> a
[2,1,3]
```

<br>

---
<br>

* 역순으로 뒤집기 : **reverse()**
```python
>>> a = [1,2,3]
>>> a.reverse()
>>> a
[3, 2, 1]
```

<br>

---
<br>

* 위치 반환 : **index()** <br>
  index(x) : 리스트에 x가 있을 경우 x의 인덱스 번호를 알려준다.
```python
>>> a = [1,2,3]
>>> a.index(2)
1
```

<br>

---
<br>

* 개수 세기 : **count()** <br>
  count(x) : 리스트에 x가 몇 개 있는지를 반환
```python
>>> a = [1,2,3,1,1]
>>> a.count(1)
3
```
<br>

## list comprehension

출력표현식 : [식 for 변수 in 리스트 if 조건식]

```python
>>> a = [ b*2 for b in range(5) if b%2 == 0]
>>> a
[0, 4, 8]
```