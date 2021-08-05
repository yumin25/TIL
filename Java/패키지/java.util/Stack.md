## Stack

```java
import java.util.Stack;
```
<br>

객체 생성
```java
Stack<Character> stack = new Stack<>();
```

<br>

* push() : 값 추가
```java
stack.push('a');
```

<br>

* pop() : 스택의 가장 위에 있는 값 삭제
```java
stack.pop();
```

<br>

* peek() : 스택의 가장 위에 있는 값 리턴
```java
stack.peek();
```

<br>

* clear() : 스택 초기화
```java
stack.clear();
```

<br>

* contains() : 값을 스택 안에서 찾은 뒤 있으면 true 반환
```java
System.out.println(stack.contains('a'));
```