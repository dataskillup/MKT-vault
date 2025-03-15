---
meeting date: <% tp.file.creation_date() %>
type: meeting
company: 
method: 
location: 
summary: 
phone: 
tags: 
Win?: false
---
tags:: #meeting 
Date: [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
<% await tp.file.rename(tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]

**Attendees**: 
- 

## Agenda/Questions


## Notes
-