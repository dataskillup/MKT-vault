---
company: 
location: 
title: 
email: 
website: 
aliases: 
relationships:
---

tags:: #contact # 
Date:: [[2025-03-12-Wednesday]]

# [[Test Person 2]]
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