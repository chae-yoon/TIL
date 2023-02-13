# Filtering Data

## DISTINCT Syntax

- 조회 결과에서 중복된 Record 제거
- SELECT 키워드 바로 뒤에 위치
- SELECT DISTINCT 키워드 다음 고유한 값을 선택하려는 하나 이상의 Field 지정

```sql
SELECT DISTINCT
  select_list
FROM
  table_name;
```

<br>

## WHERE Syntax

- FROM clause 뒤에 위치
- search_condition은 비교연산자 및 논리연산자(AND, OR, NOT 등)를 사용

```sql
SELECT
  select_list
FROM
  table_name
WHERE
  search_condition;
```

<br>

### Comparison Operators

- ex. =, >=, <=, !=, IS, LIKE, IN, BETWEEN ... AND ect.

#### LIKE

- 값이 특정 패턴에 일치하는지 확인 with `Wildcards`
- Wildcard Characters
  - `%` : 0개 이상의 문자열과 일치하는지 확인
  - `_` : 단일 문자와 일치하는지 확인

```sql
SELECT
  select_list
FROM
  table_name
WHERE
  -- word로 끝나는 경우
  select_list LIKE '%word';

  -- 4자리면서 y로 끝나는 경우
  select_list LIKE '___y';
```

<br>

#### IN (A, B, C)

- A 또는 B 또는 C인 값을 표현
- 값이 특정 목록 안에 있는지 확인

```sql
SELECT
  select_list
FROM
  table_name
WHERE
  select_list IN(A, B, C);

-- 동일 코드
WHERE
  select_list = A
  OR select_list = B
  OR select_list = C;
```

<br>

#### NOT IN (A, B, C)

- A 또는 B 또는 C가 아닌 값을 표현

```sql
SELECT
  select_list
FROM
  table_name
WHERE
  select_list NOT IN(A, B, C);

-- 동일 코드
WHERE
  select_list != A
  OR select_list != B
  OR select_list != C;
```

<br>

#### BETWEEN [A] AND [B]

- A와 B를 포함한 사이 값을 표현

```sql
SELECT
  select_list
FROM
  table_name
WHERE
  select_list BETWEEN A AND B;

-- 동일 코드
WHERE
  select_list >= A
  AND select_list <= B;

```

<br>

### Logical Operators

- ex. AND(&&), OR(||), NOT(!)

<br>

## LIMIT Syntax

- 조회하는 Record 수 제한
- LIMIT clause는 하나 또는 두 개의 인자 사용 (0 또는 양의 정수)
- row_count는 조회할 최대 Record 수 지정

```sql
SELECT
  select_list
FROM
  table_name
LIMIT [offset,] row_count;

-- 동일 코드
LIMIT row_count OFFSET [offset];
```
