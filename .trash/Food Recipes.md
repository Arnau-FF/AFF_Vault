
>[!Properties]- `$= dv.current().Parent` 
>Version:: 1
>Creation: `=dateformat(this.file.ctime,"yyyy.MM.dd - HH:mm" )`
>Last modified:  `=dateformat(this.file.mtime, "yyyy.MM.dd - HH:mm")`
>Parent:: [[00 Notes/04 Health/04 Health]]

#Notes #MOC/4
___
```button
name +
type command
action Templater: Insert Templates/Notes/MOC5/Template_First_Child.md

```
>[!Multi-Column]
>>[!Notes] Notes
>>```dataview
>>list
>>From  [[]] and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key
>>
>>```
>
>>[!Resourses] Resourses
>>```dataview
>>list
>>From   [[]] and  !#template and #Notes and #Resourse
>>
>>```
>
>>[!Project] Projects
>>```dataview
>>list
>>From   [[]]  and !#template and #Notes and #Project 
>>
>>```
>
>>[!Key] Key
>>```dataview
>>list
>>From   [[]]  and !#template and #Notes  and #Key
>>
>>```
>
>>[!Archive] Archive
>>```dataview
>>list
>>From   [[]]  and !#template and #Notes and #Archive 
>>
>>```

# Summary: