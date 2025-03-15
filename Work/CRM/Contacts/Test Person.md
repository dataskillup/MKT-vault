---
company: Test Company
location: 
title: 
email: 
website: 
aliases: 
relationships:
---

tags:: #contact # 
Date:: [[2025-03-12-Wednesday]]

# [[Test Person]]
## Notes
- 

## Meetings
```dataview
TABLE file.cday as Created, summary AS "Summary"
FROM "CRM/Meetings" where contains(file.outlinks, [[]])
SORT file.cday DESC
```
```dataview
TABLE 
   (date(now)) - date(file.ctime) AS "Last Contacted"
WHERE contains(file.tags, "meeting") OR contains(file.tags, "comm")
SORT file.ctime DESC
LIMIT 1
```