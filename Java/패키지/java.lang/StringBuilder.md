## StringBuilder, StringBuffer

문자열은 값을 변경할 수 없어 새로운 값을 할당할 때마다 새로 생성을 하지만 StringBuilder는 문자열을 버퍼에 담아 그 안에서 작업을 수행한다.<br>
StringBuilder는 단일 스레드, StringBuffer는 멀티 스레드에서 많이 사용한다.
<br><br>

객체 생성

```java
StringBuilder sb = new StringBuilder();
```

<br>

- append() : 문자열 더하기

```java
sb.append("Hello ");
```

<br>

- reverse() : 문자열 뒤집기

```java
sb.reverse();
```

<br>

- insert(index, x) : 특정 인덱스에 값 삽입

```java
sb.insert(1, 'e');
```

<br>

- length() : 길이 구하기

```java
sb.length();
```
