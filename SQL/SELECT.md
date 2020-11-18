# SELECT
<br>

#### 데이터베이스에 들어있는 데이터를 조회하기 위한 명령어

예시)
```sql
SELECT column1, column2 FROM table_name;
```
<br>

### **ALL / DISTINCT**
<br>

#### ALL :  Default이며 생략 가능한 키워드이다.
#### DISTINCT : 중복된 레코드 제거
<br>

예시)
```sql
SELECT DISTINCT column1, column2 FROM table_name;
```
<br>

### **ORDER BY**
<br>

#### 오름차순 또는 내림차순으로 데이터를 정렬
예시)
```sql
SELECT column1, column2 FROM table_name
ORDER BY column1;
```
<br>

- 만약 여러 기준으로 정렬하고자 할 경우 조건 뒤에 이어서 작성하면 된다.<br>
예시)
```sql
SELECT column1, column2 FROM table_name
ORDER BY column1, column2 DESC;
```
<br>

### **상위 n개의 데이터 조회**
<br>

- MySQL : LIMIT 시작할 지점, 출력 데이터 개수
```sql
SELECT column1, column2 FROM table_name
LIMIT 0,n;
```
<br>

- ORACLE : rownum <=n
```sql
SELECT column1, column2 FROM table_name
rownum <=n;
```
<br>

- SQL Server : TOP n
```sql
SELECT TOP n column1, column2 FROM table_name;
```