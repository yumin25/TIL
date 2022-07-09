## StringBuilder, StringBuffer

문자열은 값을 변경할 수 없어 새로운 값을 할당할 때마다 새로 생성을 하지만 StringBuilder는 문자열을 버퍼에 담아 그 안에서 작업을 수행한다.<br>
StringBuilder는 단일 스레드, StringBuffer는 멀티 스레드에서 많이 사용한다.
<br><br>

객체 생성

```java
StringBuilder sb = new StringBuilder("1234521");
```

<br>

- append() : 문자열 더하기

```java
sb.append("Hello ");    //	1234521Hello
```

<br>

- insert(int index, x) : 특정 인덱스에 값 삽입

```java
sb.insert(1, 'e');  //1e234521
```

<br>

- length() : 길이 구하기

```java
sb.length();    //7
```

<br>

- substring() : 문자열 자르기
  - substring(int index) : 해당 위치부터 이후의 모든 문자열 리턴
  - substring(int start, int end+1) : start부터 end까지의 문자열 리턴

```java
sb.substring(4);    //521
sb.substring(1,3);  //23
```

<br>

- delete(int start, int end+1) : 문자열 제거

```java
sb.delete(2,4); //12521
```

<br>

- reverse() : 문자열 뒤집기

```java
sb.reverse();   //1254321
```

<br>

- replace(int start, int end+1, String str) : 데이터 교체

```java
sb.replace(2, 5, "HH"); // 12HH21
```

<br>

- setCharAt(int index, char c) : 특정 위치의 문자 변경

```java
sb.setCharAt(2, 'q'); // 12q4521
```

<br>

- indexOf : 처음 발견되는 인덱스 반환

```java
sb.indexOf("2");    //1
sb.indexOf("8");    //-1
```

<br>

- lastIndexOf() : 뒤에서부터 시작하여 처음 발견되는 인덱스 반환

```java
sb.lastIndexOf("2");    //5
sb.lastIndexOf("8");    //-1
```
