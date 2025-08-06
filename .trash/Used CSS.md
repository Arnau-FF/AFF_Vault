
>[!Properties]- `$= dv.current().Parent` 
>Version:: 1.1
>Creation: `=dateformat(this.file.ctime,"yyyy.MM.dd - HH:mm" )`
>Last modified:  `=dateformat(this.file.mtime, "yyyy.MM.dd - HH:mm")`
>Parent:: [[00 Notes/99 Obsidian/WorkFlow/WorkFlow]]
> #Notes #MOC/5 #Resourse 
```button
name +
type command
action Templater: Insert Templates/Notes/MOC5/Template_New_Child.md

```
>[!Multi-Column]
>>[!Children] Children 
>>```dataview
>>LIST 
>>FROM "" 
>>WHERE parent = [[]] and file.name != this.file.name
>>```
>
>>[!mentioned] Mentioned On:
>>```dataview
>>List 
>>from [[]]
>>Where Parent != [[]] and file.name != this.file.name
>>```
>>
***
Sources :: 
***
# Body:











