>[!metadata]-
>```dataviewjs
>const currentFile = dv.current();
>dv.list([currentFile]);
>```
Creation:          `=dateformat(this.file.ctime,"yyyy.MM.dd - HH:mm" )`
Last Modified:  `=dateformat(this.file.mtime, "yyyy.MM.dd - HH:mm")`
