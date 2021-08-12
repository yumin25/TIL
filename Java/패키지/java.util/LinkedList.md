## LinkedList

```java
import java.util.LinkedList;
```

<br>

객체 생성
```java
LinkedList<Integer> table = new LinkedList<>();
```

<br>

* get(idx) : idx번째 값 리턴.
```java
list.get(0);
```

<br>

* add() : 기본적으로 맨 끝에 값 추가. 인덱스 지정 가능.
```java
table.add(1);
list.add(1,5);
```

<br>

* addFirst() : 맨 앞에 값 추가.
```java
list.addFirst(9);
```

<br>

* addFirst() : 맨 앞에 값 추가.
```java
list.addFirst(9);
```

<br>

* addLast() : 맨 끝에 값 추가.
```java
list.addLast(1);
```

<br>

* remove() : 기본적으로 맨 끝 값 삭제. 인덱스 지정 가능.
```java
list.remove();
list.remove(2);
```

<br>

* clear() : 리스트의 모든 값 제거.
```java
list.clear();
```

<br>

* size() : 리스트의 크기 리턴.
```java
list.size();
```

<br>

* contains() : 해당 값이 있는지 찾고 true / false로 반환.
```java
list.contains(2)
```