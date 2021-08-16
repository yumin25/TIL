## BufferedReader

버퍼를 이용해 읽는 함수이다.
읽은 데이터가 String으로 고정된다.
예외처리 또는 throws IOException을 해줘야 한다.

```java
import java.io.BufferedReader;
```

<br>

객체 생성
```java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
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

* 입력 끝까지 받기
```java
while((s=bufferedReader.readLine()) !=null) {
}
```

관련 :  [StringBuilder](https://github.com/yumin25/TIL/blob/master/Java/%ED%8C%A8%ED%82%A4%EC%A7%80/java.lang/StringBuilder.md) / 
[StringTokenizer](https://github.com/yumin25/TIL/blob/master/Java/%ED%8C%A8%ED%82%A4%EC%A7%80/java.util/StringTokenizer.md)