## 리스트 (List)

선언

```java
import java.util.ArrayList;
import java.util.Arrays;

ArrayList list = new ArrayList();
ArrayList<String> list = new ArrayList<>(Arrays.asList("One", "Two"));
```

<br>

- add : 값 추가

```java
list.add("Three");
list.add(1,"A");
```

<br>

- get : 값 가져오기

```java
System.out.println(list.get(1));     -> Two
```

<br>

- size : ArrayList 갯수 리턴

```java
System.out.println(list.size());     -> 3
```

<br>

- contains : 리스트 안에 값 존재 유무를 리턴

```java
System.out.println(list.contains("Two"));     -> true
```

<br>

- remove <br>

1. remove(인덱스) : 해당 항목 삭제, 삭제된 값 리턴<br>
2. remove(객체) :

```java
System.out.println(list.remove(1));     -> Two
```

<br>

- indexOf : 리스트에 동일한 객체가 있으면 그 인덱스를 리턴.<br>

```java
System.out.println(list.indexOf("Two"));     -> 1
```

<br>

- set : 특정 인덱스값 대체

```java
list.set(1, "Five");
```

<br>

- sort : 정렬

```java
Collections.sort(list);
```

<br>

- Stream을 사용하여 배열을 List로 변환

```java
List<Integer> list = Stream.of(배열).collect(Collectors.toList());
```

<br>

- List를 배열로 변환

```java
int[] arr = list.stream().mapToInt(i->i).toArray();
```

```java
String []arr = list.toArray(new String[list.size()]);
```

[예시](https://github.com/yumin25/algorithm/blob/master/Programmers/%EC%8A%A4%ED%83%9D_%ED%81%90/%EA%B0%99%EC%9D%80%20%EC%88%AB%EC%9E%90%EB%8A%94%20%EC%8B%AB%EC%96%B4.md)
