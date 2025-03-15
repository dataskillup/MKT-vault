---
created: <% tp.file.creation_date() %>
aliases: 
tags: 
Posts: false
Engagement: false
Outreach: false
Design: false
Win?: false
---
---
created: <% tp.file.creation_date() %>
---
tags:: #dailynotes
```widgets
type: clock
```

# <% moment(tp.file.title,'YYYY-MM-DD').format("dddd, MMMM DD, YYYY") %>

<< [[<% tp.date.now("YYYY", -1) %>/<% tp.date.now("MM-MMMM", -1) %>/<% tp.date.now("YYYY-MM-DD-dddd", -1) %>|Yesterday]] | [[<% tp.date.now("YYYY", 1) %>/<% tp.date.now("MM-MMMM", 1) %>/<% tp.date.now("YYYY-MM-DD-dddd", 1) %>|Tomorrow]] >>

---
###  Daily Questions

#####  Morning Checklist 
- [ ] Check Facebook Analytics
- [ ] Post
- [ ] Check LinkedIn
- [ ] Engage
- [ ] Research Blog/Newsletter Topics
- [ ] Check Website Analytics
- [ ] Enter Analytics Data into Obsidian
- [ ] Review Content Schedule
- [ ] Review Content Catalogue
- [ ] Daily Note

#####  Today, at work I plan to...
- 
#####  Items from yesterday that need addressing...
- 
#####  One thing I'm excited about right now is...
- 

#####  One thing I planned to accomplish today was...
- [ ] 

#####  One thing I'm struggling with today is...
- 

---
# 📝 Review
- <% tp.file.cursor() %>

---
### Notes created today
```dataview
List FROM "" 
WHERE file.path != this.file.path
AND
file.cday = this.file.cday
```

### Notes last touched today
```dataview
List FROM "" 
WHERE file.path != this.file.path
AND
file.mday = this.file.cday
```