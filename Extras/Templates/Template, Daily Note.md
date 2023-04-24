---
created: <% tp.file.creation_date() %>
---
tags:: #log/journal 

# <% moment(tp.file.title,'YYYY-MM-DD').format("dddd, MMMM DD, YYYY") %>

<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').subtract(1, 'd').format('YYYY-MM-DD-dddd') %>|Yesterday]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').add(1, 'd').format('YYYY-MM-DD-dddd') %>|Tomorrow]] >>

---
# Notes
- <% tp.file.cursor() %>

---
### Notes created today
```dataview
List FROM "" and -"Templates"
WHERE file.cday = date(" <%tp.date.now("YYYY-MM-DD")%> ") 
SORT file.ctime asc
```

### Notes last touched today
```dataview
List FROM "" WHERE file.mday = date("<%tp.date.now("YYYY-MM-DD")%>") SORT file.mtime asc
```