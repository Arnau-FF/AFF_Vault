

>[!Properties]- `$= dv.current().Parent` 
>Version:: 1
>Creation: `=dateformat(this.file.ctime,"yyyy.MM.dd - HH:mm" )`
>Last modified:  `=dateformat(this.file.mtime, "yyyy.MM.dd - HH:mm")`
>Parent:: [[My Music]]

#Notes 
***
```button
name +
type command
action Templater: Insert Templates/Notes/MOC5/Template_New_Child.md

```
>[!Multi-Column]
>>[!brother]
>>```dataview
>>list
>>From !#moc/5
>>WHERE contains(parent, this.parent) and file.name != this.file.name
>>limit 10
>>```
>
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





