## WHERE
<br>

#### 레코드를 필터링하기 위한 명령어
#### 조건을 만족하는 레코드만 필터링해서 보여준다.

예시)
```sql
SELECT column1, column2
FROM table_name
WHERE condition;
```

### 연산자
* AND
* OR
* NOT
<br>

예시)
```sql
SELECT column1, column2
FROM table_name
WHERE condition1 AND condition2;
```

```sql
SELECT column1, column2
FROM table_name
WHERE condition1 OR condition2;
```

```sql
SELECT column1, column2
FROM table_name
WHERE NOT condition;
```

관련 자료
[w3schools](https://www.w3schools.com/sql/sql_where.asp)