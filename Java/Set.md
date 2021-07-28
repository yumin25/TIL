## Set
중복 허용 x, 순서 x

선언
```java
Set<String> set = new HashSet<String>();
```
<br>


* add : 값 추가
```java
set.add("a");
```

<br>

* remove : 값 제거
```java
set.remove("a");
```

<br>

* isEmpty : 값 존재 유무 리턴
```java
set.isEmpty();
```

<br>

* contains : 값 포함 유뮤 리턴
```java
set.contains("a");
```

<br><br>

LinkedHashSet : 입력된 순서대로 data 정렬<br>
TreeSet : 오름차순으로 data 정렬