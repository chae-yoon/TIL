# Sorting Data

## ORDER BY Syntax

- FROM clause 뒤에 위치
- 하나 이상의 Field 기준으로 결과를 오름차순, 내림차순으로 정렬할 수 있음

  - ASC : 오름차순 (Default)
  - DESC : 내림차순
  - 여러 개의 Field인 경우 : 첫 번째 Field로 정렬 → 정렬 후 같은 Record를 다음 Field 기준으로 정렬

```sql
SELECT
  select_list
FROM
  table_name
ORDER BY
  column1 [ASC|DESC],
  column2 [ASC|DESC],
  ...;
```
