---
Teeth: false
Runing: false
gym: false
Flexibility: false
obsidian: false
learn: false
teeth: false
runing: false
---
# {{date:dddd, MMMM Do, YYYY}}
>[!Properties]- | [[{{yesterday}}|Yesterday]] | [[{{tomorrow}}|Tomorrow]] | 
>Version:: 2.1
>Parent:: [[{{date:MMMM, yyyy}}]]
>Tags: #Notes #Journal 
***
```meta-bind-embed
[[Journal_Header]]
```
<% tp.web.daily_quote() %>
# Tasks To do:
>[!Multi-Column] Physical
>>[!Task] To do 
>>```dataview
>>task from #journal
>>where !completed
>>sort file.name asc
>>```
>
>>[!Month] [[{{date:MMMM, yyyy}}]]
>>```dataview
>>task
>>WHERE file.name = "{{date:MMMM, yyyy}}"
>>```
***
## New Tasks :
- [ ]
***

# Key Notes:


# Habits:
```meta-bind-embed
[[Journal_Habits]]
```
# Foot:

>[!metadata]- 
>```dataviewjs
>const currentFile = dv.current();
>dv.list([currentFile]);
>```
Creation:          `=dateformat(this.file.ctime,"yyyy.MM.dd - HH:mm" )`
Last Modified:  `=dateformat(this.file.mtime, "yyyy.MM.dd - HH:mm")`


