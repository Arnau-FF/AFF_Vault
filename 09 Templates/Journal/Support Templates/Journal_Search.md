---
Type: 
---
>[!Multi-Column]
>>[!Children]+ Children 
>>```dataview
>>LIST 
>>FROM "" 
>>WHERE parent = [[]] and file.name != this.file.name
>>```
>
>>[!mentioned]+ Mentioned On:
>>```dataview
>>List 
>>from [[]]
>>Where Parent != [[]] and file.name != this.file.name
>>```

>[!type] Type: `INPUT[inlineSelect(option(Null),option(Link),option(Idea),option(Tool), option(Video),option(Quote),option(Knowledge),option(Redacted), option(Code),option(Example),option(Key),option(Project),option(People)):Type]`  Status: `INPUT[inlineSelect(option(Null),option(To Start), option(Paused), option(0%), option(50%), option(100%), option(To Revise)):Status]`



