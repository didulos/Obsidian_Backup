# NLP

```dataview
TABLE status as 상태
FROM "01-Terms"
WHERE contains(category, this.file.name)
SORT file.name ASC
```