>[!metadata]-
>```dataviewjs
>const currentFile = dv.current();
>dv.list([currentFile]);
>```

Creation:          `=dateformat(this.file.ctime,"yyyy.MM.dd - HH:mm" )`
Last Modified:  `=dateformat(this.file.mtime, "yyyy.MM.dd - HH:mm")`
Status: `INPUT[inlineSelect(option(Null),option(To Start), option(Paused), option(0%), option(50%), option(100%), option(To Revise)):Status]`