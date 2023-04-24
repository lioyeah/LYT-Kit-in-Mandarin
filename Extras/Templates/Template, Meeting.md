---
date: <% tp.file.creation_date() %>
type: meeting
company: 
summary: " "
---
tags: #log/meeting 
Date: [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
<% await tp.file.move("/Calendar/Meetings/" + tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]

**Attendees**: 
- 

## Agenda/Questions
- 

## Notes
-