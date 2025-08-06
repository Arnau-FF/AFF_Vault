---
Type: Note
---
>[!Multi-Column]
>>[!Children]+ Children 
>>```dataview
>>LIST 
>>FROM "" 
>>WHERE parent = [[]] and file.name != this.file.name
>>SORT Priority DESC
>>```
>
>>[!mentioned]+ Mentioned On:
>>```dataview
>>List 
>>from [[]]
>>Where Parent != [[]] and file.name != this.file.name
>>SORT Priority DESC
>>```

>[!type] Type: `INPUT[inlineSelect(option(Note,Note), option(Project), option(Resource), option(Archive)):Type]` Sub-Type: `INPUT[inlineSelect(option(Null), option(Video), option(Link), option(Idea), option(Tool), option(Link), option(To Revise),option(Key)):sub-type]` Color: `INPUT[inlineSelect(option(Null), option(Red), option(Orange), option(Yellow), option(Green), option(Blue), option(Purple), option(Pink), option(Brown), option(Grey), option(Black), option(White)):Color]` Priority: `INPUT[inlineSelect(option(9), option(8), option(7), option(6), option(5), option(4), option(3), option(2), option(1), option(0)):Priority]`
