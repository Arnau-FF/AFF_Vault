---
update_test_type: maintenance
update_tests:
- image: 0.17.0-py3
  update_test_type: simplepip
  additional: pip=21.3.1
  wip: true
  done: true
- image: 0.18.0
  channel: maintenance
  start: 1.8.7
  wip: true
  done: true
- image: 0.18.0-latest
  channel: maintenance
  wip: true
  done: true
- image: 1.0.0
  channel: maintenance
  start: 1.8.7
  wip: true
  done: true
- image: 1.0.0-latest
  channel: stable
  wip: true
  done: true
- image: 1.0.0-latest
  channel: maintenance
  start: 1.9.0rc3
  wip: true
  done: true
- image: 1.0.0-latest
  channel: maintenance
  start: 1.9.0rc4
  wip: true
  done: true


---
#Notes/Obsidian/OB_Plugins/Dataview_Plugin 

>[!header]- [[ Dataview_Plugin ]] `button-Child`  
>>[!Brothers]+ 
>>```dataview
>>List
>>From !"Templates"
>>WHERE econtains(file.etags,"#Notes/Obsidian/OB_Plugins/Dataview_Plugin") and file.name != this.file.name
>>Sort file.name ascending
>>```
***
>[!Children] 
>```dataview
>List
>From #Notes/Obsidian/OB_Plugins/Dataview_Plugin/Ex_Input_data__into_a_table 
>Sort file.name ascending
>```
***
>[!mentioned] 
>```dataview
>list
>From [[]] and !#Notes/Obsidian/OB_Plugins/Dataview_Plugin/Ex_Input_data__into_a_table
>Sort file.name ascending
> ```



 

