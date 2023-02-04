---
created: <% tp.file.creation_date() %>
---

# Person Name
Title, company, how I know them

## Open Items
```tasks
description includes <% tp.file.title %>
not done
```

## Communication Log
```dataview
table file.cday as "Created" from [[<% tp.file.title %>]]
sort file.cday DESC
```
