---
Point of Contact: Test Person
location: 
field: 
email: 
website: 
aliases:
---

tags:: #contact 
Date:: [[2025-03-12-Wednesday]]

# [[Test Company]]
## Notes
- 

## Meetings
```dataview
TABLE file.cday as Created, summary AS "Summary"
FROM "CRM/Meetings" where contains(company, this.file.name)
SORT file.cday DESC
```