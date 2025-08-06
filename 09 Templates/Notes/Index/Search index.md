
```dataview
TABLE Without ID
file.link as "Areas",
sort(filter(file.inlinks, (x) => contains(x.file.tags, "#MOC/3")), (y) => y.file.name) as "Themes"
FROM #MOC/2 and !"09 Templates"
SORT Priority ASC

```
