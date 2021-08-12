## Math

<br>

* round() : 소수점 첫번째 자리를 반올림해 정수로 리턴.
```java
double a = 1.123;
Math.round(a);    -> 1
Math.round(a*100)/100.0; -> 1.12    //소수점 둘째 자리까지 나타내기
```

<br>

* abs() : 인자값에 대한 절댓값 반환.
```java
Math.abs(a);
```

<br>

* sqrt() : 인자값에 대한 제곱근 반환.
```java
Math.sqrt(25);  -> 5.0
```

<br>

* pow(a,b) : a<sup>b</sup> 반환.
```java
Math.pow(2,5);  -> 32.0
```

<br>

* max(a,b) : a와 b 중 큰 값 반환.
```java
Math.max(2,5);  -> 5
```

<br>

* min(a,b) : a와 b 중 작은 값 반환.
```java
Math.min(2,5);  -> 2
```

<br>

* random() : 0.0 <= x < 1.0 의 실수값 리턴.

```java
Math.random();  -> 0.990386277283181
(int)(Math.random()*10)+1;    -> 1    // 1 ~ 10 中 정수값
```
Math.random() * (max-min+1) + min : min <= x <= max 리턴.