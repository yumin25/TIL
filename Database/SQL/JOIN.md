## **JOIN**

#### 두 개 이상의 테이블에서 행을 결합할 때 사용

<br>
<br>

## **INNER JOIN**

#### 두 테이블에서 일치하는 값이 있는 레코드 출력

<br>
<img src = https://user-images.githubusercontent.com/49578987/99905579-06686480-2d15-11eb-8931-fbfc9b2c217f.PNG width="150px">

예시)

```sql
SELECT table1.column2, table2.column3
FROM table1
INNER JOIN table2
ON table1.column1 = table2.column1;
```

<br>

## **LEFT OUTER JOIN**

#### 왼쪽 테이블의 모든 레코드 반환, 오른쪽 테이블에서 일치하는 값이 없을 시 NULL로 표기

<br>

<img src = https://user-images.githubusercontent.com/49578987/99905563-e3d64b80-2d14-11eb-9a7e-1cb46d7c3683.PNG width="150px">

예시)

```sql
SELECT table1.column2, table2.column3
FROM table1
LEFT JOIN table2
ON table1.column1 = table2.column1;
```

<br>

## **RIGHT OUTER JOIN**

#### 오른쪽 테이블의 모든 레코드 반환, 왼쪽 테이블에서 일치하는 값이 없을 시 NULL로 표기

<br>

<img src = https://user-images.githubusercontent.com/49578987/99905604-2ef05e80-2d15-11eb-9e1f-67c511a5007f.PNG width="150px">

예시)

```sql
SELECT table1.column2, table2.column3
FROM table1
RIGHT JOIN table2
ON table1.column1 = table2.column1;
```

<br>

## **FULL OUTER JOIN**

#### 모든 레코드를 반환한다

<br>

<img src = https://user-images.githubusercontent.com/49578987/99905633-5d6e3980-2d15-11eb-9378-686277325442.PNG width="150px">

예시)

```sql
SELECT table1.column2, table2.column3
FROM table1
FULL OUTER JOIN table2
ON table1.column1 = table2.column1;
```

<br>

## **CROSS JOIN**

#### 두 테이블 간 가능한 모든 경우의 수에 대한 결합을 출력. <br> 출력 데이터 행의 개수 : table1 행 개수 \* table2 행 개수

<br>

예시)

```sql
SELECT table1.column2, table2.column3
FROM table1
CROSS JOIN table2;
```

<br>

## **SELF JOIN**

#### 자기 스스로 결합

<br>

예시)

```sql
SELECT T1.column2, T2.column3
FROM table1 AS T1, table1 AS T2;
```

[ON](https://github.com/yumin25/TIL/blob/master/Database/SQL/ON.md)

관련 자료
[w3schools](https://www.w3schools.com/sql/sql_join.asp)
