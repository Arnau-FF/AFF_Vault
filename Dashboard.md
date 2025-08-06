>[!Properties]-  | `= this.file.link` | 
>Version:: 2.0
>Parent:: [[Dashboard]] 
>Tags: #MOC/1   

***
# [[Index]]  

>[!Multi-Column] 
>>[!Last]
>>```dataview
>>list
>>from ""  // Optional: Replace with a folder path or remove this line to search all notes
>>where file.mtime != null
>>sort file.mtime desc
>>limit 10  // Adjust the number of notes to display
>>
>>```
>
>
>>[!To Revise] To Revise
>>```dataview
>>list
>>from ""  // Optional: Replace with a folder path or remove this line to search all notes
>>where sub-type = "To Revise"
>>```
***




 
# Foot
 
```meta-bind-embed
[[Foot MOC2]]
```