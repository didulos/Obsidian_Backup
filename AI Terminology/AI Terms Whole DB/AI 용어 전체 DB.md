# AI 용어 전체 DB

```dataview
TABLE 
  category as 분야,
  status as 상태,
  file.size as 크기
FROM "Terms"
WHERE type = "term"
SORT category ASC
```