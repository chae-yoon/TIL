# Grouping Data

## GROUP BY Syntax

- 집계 함수와 함께 Record를 그룹화하여 요약본 생성
  - `Aggregation Funcions(집계 함수)` : 값에 대한 계산을 수행하고 단일한 값을 반환하는 함수
  - SUM, AVG, MAX, MIN, COUNT
- FROM 및 WHERE 절 뒤에 배치
- GROUP BY 절 뒤에 그룹화할 필드 목록 작성
- `HAVING` clause로 집계 항목에 대한 세부 조건 지정 가능

```sql
SELECT
  c1, c2, ..., cn, aggregate_function(ci)
FROM
  table_name
GROUP BY
  c1, c2, ..., cn
HAVING
  search_condition;
```
