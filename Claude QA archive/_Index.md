# Claude QA Archive — Index

> Dataview 플러그인 설치 시 자동 활성화.
> 미설치 상태에서는 코드블록으로 보입니다.

## 최근 30일

```dataview
TABLE date, topic, tags
FROM "Inbox"
WHERE date >= date(today) - dur(30 days)
SORT date DESC
```

## 토픽별 묶음

```dataview
TABLE rows.file.link AS notes
FROM "Inbox"
GROUP BY topic
```

## Better Ask 모음 (프롬프트 진화 노트)

```dataview
LIST file.link
FROM "Inbox"
SORT date DESC
LIMIT 50
```
