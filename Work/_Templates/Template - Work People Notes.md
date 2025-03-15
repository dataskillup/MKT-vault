---
type: person
company: 
location: 
title: 
email: 
website: 
aliases: 
relationships:
---

tags:: #contact 
Date:: [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
<% await tp.file.rename(tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]
## Notes
- 

## Meetings
```dataview
TABLE file.cday as Created, summary AS "Summary"
FROM "CRM/Meetings" where contains(file.outlinks, [[]])
SORT file.cday DESC
```

## Last Contact
```dataview
TABLE WITHOUT ID
   (date(now)) - date(file.mtime) AS "Last Contacted"
WHERE contains(file.tags, "meeting")
SORT file.mtime DESC
LIMIT 1
```