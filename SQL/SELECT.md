## SELECT
<br>

#### 데이터베이스에 들어있는 데이터를 조회하기 위한 명령어

예시)
```sql
SELECT column1, column2 FROM table_name;
```
<br>

### ALL / DISTINCT
<br>

#### ALL :  Default이며 생략 가능한 키워드이다.
#### DISTINCT : 중복된 레코드 제거

예시)
```sql
SELECT DISTINCT column1, column2 FROM table_name;
```
<br>

### ORDER BY
<br>

#### 오름차순 또는 내림차순으로 데이터를 정렬
예시)
```sql
SELECT column1, column2 FROM table_name
ORDER BY column1;
```