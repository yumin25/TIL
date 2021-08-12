## String

<br>

* toCharArray() : 한 글자씩 char 타입 배열에 넣는다.
```java
char []ch = br.readLine().toCharArray();
```

<br>

* charAt(int index) : index번째 문자 리턴.
```java
System.out.println(word.charAt(2));
```

<br>

* length() : 문자열 길이 리턴.
```java
System.out.println(word.length());
```

<br>

* indexOf(String str) : str의 index값 리턴. 없을 시 -1 리턴.
```java
System.out.println(word.indexOf('d'));
```

<br>

* lastIndexOf(String str) : str를 끝에서부터 찾아 index값 리턴. 없을 시 -1 리턴.
```java
System.out.println(word.lastIndexOf('s'));
```

<br>

* toUpperCase() : 모두 대문자로 변경
```java
System.out.println(word.toUpperCase());
```

<br>

* toLowerCase() : 모두 소문자로 변경
```java
System.out.println(word.toLowerCase());
```

<br>

* contains() : 특정 문자열이 포함되어 있으면 true 리턴.
```java
System.out.println(word.contains("aa"));
```