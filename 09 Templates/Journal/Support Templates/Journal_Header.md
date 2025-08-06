>[!Multi-Column]
>>[!Time] 
>>```dataviewjs
>>const startDate = moment("1995-11-16"); // Replace with your start date
>>const endDate = moment("2080-12-31"); // Replace with your end date
>>const currentDate = moment(); // Current date
>>
>>const totalDuration = endDate.diff(startDate, "days"); // Total duration in days
>>const elapsedTime = currentDate.diff(startDate, "days"); // Elapsed time in days
>>
>>// Calculate progress percentage
>>const progressPercentage = (elapsedTime / totalDuration) * 100;
>>
>>// Clamp the progress to be between 0 and 100
>>const clampedProgress = Math.min(Math.max(progressPercentage, 0), 100);
>>
>>// Create the progress bar and the percentage text
>>const progressBar = `<progress value="${clampedProgress}" max="100"></progress><br>`;
>>const progressText = `${Math.round(clampedProgress)}% completed`;
>>
>>// Output the progress bar and the text
>>dv.span(progressBar + progressText);
>
>>[!Birthday] 🎂
>>```dataview
>>LIST WITHOUT ID 
>>link(file.name, file.name + " (" + round((date(now) - birthday).years, 0) + ")")
>>FROM ""
>>WHERE 
>>    date(birthday).month = date(now).month AND
>>    date(birthday).day >= date(now).day AND
>>    date(birthday).day <= date(now).day + 3
>>SORT date(birthday).day ASC
>>```

