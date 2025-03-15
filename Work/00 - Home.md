---
banner: "[[banner.jpg]]"
banner-y: 50
content-start: 100
banner-display: cover
banner-repeat: true
banner-height: 250
banner-fade: -100
banner-radius: 500
banner-inline-title-color: "#f7da97"
---
```widgets
type: clock
format: 12hr
```
>[!info] Weblinks+
>Aggregate your organization weblinks here, for easy access in communications, along with your preferred LLM.
>
>webpage:
>Facebook:
>Instagram: 
>LinkedIn: 
>Alignable: 
>Web Admin Panel:
>Gemini: [gemini.google.com]() 
>

`BUTTON[persons, company, meetings, comm, project, idea]`


> [!summary]+ Contact
> Dataview query to show contacts from CRM with their related organization and relationship to you. Buttons at the top can be used to add new entries.
> 
> 
> 
>```dataview
>TABLE  file.cday as "Created", company as "Org", relationship as "Status"
>FROM "CRM/Contacts"
>SORT DESC
>```

> [!warning]+ Recent Interactions
> Aggregates meeting and communication notes to show the last 10 recent interactions, sorted by most recent. Use the following buttons to create a new note  of the related type.
> 
>  > 
>   ```dataview
>   TABLE  file.cday as "Created", summary as "Summary"
>   FROM "CRM/Meetings" OR "CRM/Communications"
>  SORT file.cday DESC
>  LIMIT 10
>  ```

>[!tldr]+ Current Projects
>Dataview query to list all open projects with a link to their associated file. Create a new project: using the following meta-bind button:
>
>>
>```dataview
>TABLE file.cday as "Created", file.folder as "Status", summary as "Summary", Budget as "Budget", Actual as "Actual" 
>FROM "Projects"
>SORT file.folder ASC
>LIMIT 5
>```

>[!note]+ Tasks
>
>Aggregated tasks from across all note sources, sorted by date. 
>```tasks
>not done
>```
>




>[!success]+ Wins
>Completed projects, tasks, and content that performed well. Denoted in frontmatter as a Win
>
>```dataview
>LIST
>WHERE file.folder = "CRM"
>OR file.folder = "Projects" 
>OR file.folder = "Content" 
>OR file.folder = "Rituals" 
>OR contains(file.path, "CRM/") 
>OR contains(file.path, "Projects/") 
>OR contains(file.path, "Content/") 
>OR contains(file.path, "Rituals/") 
>AND Win = true
>SORT Desc 
>LIMIT 5 
>```


>[!hint]+ Content Ideas
>Dataview query to aggregate all content ideas, sorted by most recent. Use the meta-bind button below to log a new content idea.
>
>  
>
>```dataview
>TABLE file.cday as "Created", summary as "Summary", medium as "Medium", platform as "Platform"
>FROM "Content"
>SORT file.cday DESC
>```

>[!abstract] Work Recap
>```dataview
>TABLE file.cday as Created
>FROM "Rituals"
>LIMIT 7
>```




# Analytics

This section aggregates the various trackers from the `trackers` plugin. Using this plugin, you can create fairly in-depth data visualizations. I've included some simple examples to illustrate.

![[Project Costs Tracker]] ![[Project Budget Tracker]]