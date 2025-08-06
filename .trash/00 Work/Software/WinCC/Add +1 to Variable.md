---
Status: To Revise
---
# `= this.file.link`
>[!Properties]- | `= this.Parent.Parent.Parent.Parent` |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` |`BUTTON[note]` 
>Version:: 2.0
>Parent:: [[WinCC]]
>Tags: #Notes
```meta-bind-embed
[[Search note]]
```
Source::
***
# Body
Adds +1 to a variable coming form PLC without the need to define a new variable. 
```
'Visual addition of +1 to the value of DBC Program number to correspond with Number diplayed on roland Screen. 

'Declaration
Dim  ActualOld
Dim  ActualNew


Set ActualOld =HmiRuntime.SmartTags("FOL_Roland_1_Inputs_ActProgNumber")
Set ActualNew =HmiRuntime.SmartTags("_DBC1_Actual_Pgrm_Nbr")

'Addition
ActualNew.Value = ActualOld.Value + 1 

```

If the Script is used on a Variable Value Change event, the variable must be used in some screen in order to be looked at it by smart tags. A work a round is to call the script from the Variable Value Change event and the Screen load event where you want to see the new value


Used in Voestalpine








# Foot
```meta-bind-embed
[[Foot note]]
``` 