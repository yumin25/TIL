## PriorityQueue

```java
import java.util.PriorityQueue;
```

<br>

<h3>특징</h3>

1. 높은 우선순위의 요소가 먼저 나옴 (들어간 순서와 상관 X)
2. 힙으로 구현

<br>

객체 생성

```java
// 낮은 숫자 우선
PriorityQueue<Integer> priorityQueue = new PriorityQueue<>();
// 높은 숫자 우선
PriorityQueue<Integer> priorityQueue = new PriorityQueue<>(Collections.reverseOrder());
```

<br>

- add() : 값 추가. 성공 시 true 반환, 실패할 시 IllegalStateException 발생

```java
priorityQueue.add(1);
```

<br>

시간복잡도 : O(n𝑙𝑜𝑔𝑛)

<br>

관련 예시 : [백준 10814 나이순 정렬](https://github.com/yumin25/algorithm/blob/master/boj/%EC%A0%95%EB%A0%AC/10814%20%EB%82%98%EC%9D%B4%EC%88%9C%20%EC%A0%95%EB%A0%AC.md)
