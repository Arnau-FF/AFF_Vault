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

>[!type] Type: `INPUT[inlineSelect(option(Null),option(Link),option(Idea),option(Tool), option(Video),option(Quote),option(Knowledge),option(Redacted), option(Code),option(Example),option(Key),option(Project),option(People)):Type]`  Status: `INPUT[inlineSelect(option(Null), option(Paused), option(0%), option(50%), option(100%), option(To Revise)):Status]` Priority: `INPUT[inlineSelect(option(9), option(8), option(7), option(6), option(5), option(4), option(3), option(2), option(1), option(0)):Priority]`




