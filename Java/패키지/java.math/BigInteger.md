## BigInteger
문자열 형태. 숫자의 범위가 무한이다.

<br>

선언
```java
import java.math.BigInteger;

BigInteger b = new BigInteger("1000");
```
<br>

* add : 더하기
```java
b.add(c);
```

<br>

* subtract : 빼기
```java
b.subtract(c)
```

<br>

* multiply : 곱하기
```java
b.multiply(c);
```

<br>

* divide : 나누기
```java
b.divide(c);
```

<br>

* remainder : 나머지
```java
b.remainder(c);
```

<br><br>


### 형 변환
<br>

```java
// int -> BigInteger
BigInteger b = BigInteger.valueOf(1000);

// BigInteger -> int
int a = b.intValue();
```
intValue / longValue / floatValue / doubleValue / toString
<br>
