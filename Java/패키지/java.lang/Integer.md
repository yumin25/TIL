## Integer

<br>

- 진수 변환
  - toBinaryString(i) : 10진수를 2진수 문자열로 변환
  - toOctalString(i) : 10진수를 8진수 문자열로 변환
  - toHexaString(i) : 10진수를 16진수 문자열로 변환

```java
String a = Integer.toBinaryString(11);
```

- parseInt() : 문자열을 10진수로 변환. 2, 8, 16진수도 10진수로 변환 가능하다.

```java
int a = Integer.parseInt("1001",2);
```
