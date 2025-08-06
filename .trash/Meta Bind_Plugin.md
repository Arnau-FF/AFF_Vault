---
toggle: false
slider2: -20
select: option 3
multiSelect: 
date1: 2023-05-17
date2: 2023-05-17
editor: ""
suggest: option 2
fileSuggest: Casa el Josep|Casa el Josep
---
#Notes/Obsidian/OB_Plugins  #Type/Plugin/Funtionality 
>[!header]- [[ OB_Plugins ]] `button-Child`  
>>[!Brothers]+ 
>>```dataview
>>List
>>From !"Templates"
>>WHERE econtains(file.etags,"#Notes/Obsidian/OB_Plugins") and file.name != this.file.name
>>Sort file.name ascending
>>```
***
>[!Children] 
>```dataview
>List
>From #Notes/Obsidian/OB_Plugins/Meta_Bind__Plugin 
>Sort file.name ascending
>```
***
>[!mentioned] 
>```dataview
>list
>From [[]] and !#Notes/Obsidian/OB_Plugins/Meta_Bind__Plugin 
>Sort file.name ascending
> ```

