## Scanner
읽은 바이트를 문자, 정수, 실수, 문자열 등 다양한 타입으로 변환하여 리턴하는 클래스

```java
import java.util.Scanner;
```
<br>

객체 생성
```java
Scanner scanner = new Scanner(System.in);
```

<br>

* nextLine() : 한 줄 리턴. \n을 포함하는 한 줄을 읽고 \n을 제외한 나머지만 리턴.
```java
String a = scanner.nextLine();
```
aa bb cc 입력 시 aa bb cc 리턴

<br>

* next() : 화이트 스페이스를 기준으로 문자열 리턴.
```java
String a = scanner.next();
```
aa bb cc 입력 시 aa 리턴

<br>

* nextInt() : int 타입으로 리턴
```java
int a = scanner.nextInt();
```
11 22 33 입력 시 11 리턴

<br>

* char 입력받기
```java
char a = scanner.next().charAt(0);
```
next()로 문자열을 입력받은 뒤 charAt(0)으로 첫번째 문자 꺼냄.