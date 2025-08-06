
>[!Multi-Column] Physical
>>[!Task] To do 
>>```dataview
>>task from "00 Notes/01 Arnau/To Remember/Journal/2024/Daily"
>>where !completed
>>```
>
>>[!Month] [[{{date:MMMM, yyyy}}]]
>>```dataview
>>task
>>WHERE file.name = "{{date:MMMM, yyyy}}"
>>```
>