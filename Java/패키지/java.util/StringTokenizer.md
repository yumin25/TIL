## StringTokenizer

문자열을 구분자로 쪼개주는 함수

```java
import java.util.StringTokenizer;
```

<br>

객체 생성
```java
StringTokenizer st = new StringTokenizer("ab cd");
```

<br>

* readLine() :  한 줄 읽기.
    -  Integer.parseInt : int로 읽기 위해서는 형변환이 필수이다.
    - toCharArray : 한 글자씩 char 배열에 입력.
```java
int a = Integer.parseInt(br.readLine());
char a[] = br.readLine().toCharArray();
```

<br>

* nextToken : 다음 토큰 반환

<br>

* hasMoreTokens : 사용할 토큰이 더 있는지 확인.
```java
while(st.hasMoreTokens()) {
	System.out.println(st.nextToken());
}
```

<br>