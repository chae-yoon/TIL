# SELECT Statement

## SELECT Syntax

- 테이블의 데이터를 조회 및 반환
- SELECT 키워드 다음에 데이터를 선택하려는 Field를 하나 이상 지정 (모든 필드 데이터인 경우 `*`)
- FROM 키워드 다음에 데이터를 선택하려는 테이블의 이름을 지정
- 기본적인 사칙연산 사용 가능

```sql
SELECT
  select_list
FROM
  table_name;
```

<br>

## AS Keyword

- 필드에 새로운 별칭을 지정

```sql
SELECT
  select_list AS keyword
FROM
  table_name;
```

<br>

## SELECT Statement 실행 순서

- 테이블에서 특정 조건에 맞춰 그룹화 하고 만약 그룹 중에서 조건이 있다면 필터링 한 뒤 조회하여 정렬해 특정 위치의 값을 출력

1. FROM
2. WHERE
3. GROUP BY
4. HAVING
5. SELECT
6. ORDER BY
7. LIMIT
