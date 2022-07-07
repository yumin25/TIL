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

* ROLLUP &nbsp;:&nbsp; GROUP BY에서 선택한 기준에 따라 합계가 구해진다.<br>
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
