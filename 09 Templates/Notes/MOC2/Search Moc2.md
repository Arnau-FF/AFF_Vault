
>[!Children]+ Moc3
>```dataview
>LIST 
>FROM "" 
>WHERE parent = [[]] and file.name != this.file.name
>SORT Priority DESC
>```

>[!type] Priority: `INPUT[inlineSelect(option(9), option(8), option(7), option(6), option(5), option(4), option(3), option(2), option(1), option(0)):Priority]`