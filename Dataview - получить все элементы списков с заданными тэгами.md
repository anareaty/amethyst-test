---
date: 2024-04-14
cssclasses:
  - note
Тип: запрос
Раздел: "[[Запросы]]"
---


## Текст:
- строка 1 \#тэг1 \#тэг2
- строка 2 \#тэг1 \#тэг3
- строка 3 \#тэг2 \#тэг3
- [h] строка 4 \#тэг1 \#тэг2


## Запрос:
````
```dataview
list without id

L.text

from #тэг1 and #тэг2 

flatten file.lists as L

where contains(L.tags, "тэг1") and contains(L.tags, "тэг2")
```
````

