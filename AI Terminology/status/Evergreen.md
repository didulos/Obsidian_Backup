# Evergreen (파악이 된 용어)

```dataview
TABLE category as 분야
FROM "01-Terms"
WHERE status = "evergreen"
SORT file.name ASC
```