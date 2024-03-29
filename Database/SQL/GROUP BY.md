# GROUP BY

<br>

#### 특정 속성의 값이 같은 튜플들을 모아 그룹화하는 명령어

<br>

예시)

```sql
SELECT column1, column2
FROM table_name
GROUP BY column1;
```

<br>

- ROLLUP &nbsp;:&nbsp; GROUP BY에서 선택한 기준에 따라 합계가 구해진다.<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  MYSQL은 WITH ROLLUP<br>

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;보통의 SELECT된 데이터와 그 데이터의 총계<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  NULL로 묶어 표현
  <br>

예시)

```sql
SELECT column1, column2, SUM(column1)
FROM table_name
GROUP BY ROLLUP(column1, column2);
```

<br>

## HAVING

group by된 이후 특정한 필드로 그룹화 되어진 새로운 테이블에 조건을 줄 수 있다.<br>
집계함수를 가지고 조건비교를 할 때 사용.
