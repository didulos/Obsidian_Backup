# Computet-Vision

```dataview
TABLE status as 상태
FROM "Terms"
WHERE contains(category, replace(this.file.name, "Cat-", ""))
SORT file.name ASC
```