
```dataview
TABLE Without ID
file.link as "  ",
sort(filter(file.inlinks, (x) => contains(x.file.tags, "#MOC/4")), (y) => y.file.name) as ""
FROM #MOC/3 and #Notes and !#template and !"09 Templates"
SORT file.name ASC

```

``` dataview
TABLE Without ID
sort(filter(file.outlinks, (x) => contains(x.file.tags, "#MOC/3")), (y) => y.file.name) as "MOC/3",
file.link as "MOC/4",
sort(filter(file.inlinks, (x) => contains(x.file.tags, "#MOC/5")), (z) => z.file.name) as "MOC/5"
FROM #MOC/4 and #Notes and !#template and "00 Notes"
SORT file.name ASC

```