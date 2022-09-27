## Queue

LinkedList를 활용

```java
import java.util.LinkedList;
import java.util.Queue;
```

<br>

객체 생성

```java
Queue<Character> queue = new LinkedList<>();
```

<br>

- add() : 값 추가. 값 추가 실패 시 illegalStateException 발생.

```java
queue.add('a');
```

<br>

- offer() : 값 추가. 값 추가 실패 시 false 반환.

```java
queue.offer('a');
```

<br>

- poll() : 큐의 첫번째 값 삭제. 큐가 비어있으면 null 반환.

```java
queue.poll();
```

<br>

- remove() : 큐의 첫번째 값 삭제. 큐가 비어있으면 NoSuchElementException 발생.

```java
queue.remove();
```

<br>

- peek() : queue의 첫번째 값 리턴.

```java
queue.peek();
```

- [PriorityQueue](https://github.com/yumin25/TIL/blob/master/Java/%ED%8C%A8%ED%82%A4%EC%A7%80/java.util/PriorityQueue.md)
