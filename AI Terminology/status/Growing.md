# Growing (조금 개념을 파악)

```dataview
TABLE category as 분야
FROM "Terms"
WHERE status = "growing"
SORT file.name ASC
```