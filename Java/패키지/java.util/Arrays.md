## Arrays
배열 다루는 함수들
```java
import java.util.Arrays;
```
<br>

* toString : 배열 값 출력. 일차원 배열 출력할 때 사용.

```java
System.out.println(Arrays.toString(map));
```

<br>

* sort : 오름차순 정렬

```java
Arrays.sort(map);
```

<br>

* fill : 배열의 모든 값을 특정 값으로 초기화

```java
Arrays.fill(map,1);
```

<br>

* deepToString : 다차원 배열 출력.
```java
import java.util.Arrays;

int[][] num = {{1,2,3,4}, {5,6,7,8}};
System.out.println(Arrays.deepToString(num));

[[1, 2, 3, 4], [5, 6, 7, 8]]
```

<br>

* arraycopy : 배열 복사
```java
int [] a = {1,2,3,4};
int [] b = new int[8];
System.arraycopy(a, 0, b, 4, a.length);
System.out.println(Arrays.toString(b));

[0, 0, 0, 0, 1, 2, 3, 4]

```

<br>