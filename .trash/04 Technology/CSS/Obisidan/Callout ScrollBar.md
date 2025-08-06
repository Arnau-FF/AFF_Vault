# `= this.file.link`
>[!Properties]- | `= this.Parent.Parent.Parent.Parent` |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` |`BUTTON[note]` 
>Version:: 2.1
>Parent:: [[Callouts]]
>Tags: #Notes
```meta-bind-embed
[[Search note]]
```
Source::
Related To::
***
# Body:

Looks for any callout with 30 on it➔ [!any callout|30]
Fixes height of callout and adds scroll bar.
```
.callout[data-callout-metadata="30"] {

    max-height: 32vh;

    overflow: scroll;

  

}
```






# Foot
```meta-bind-embed
[[Foot note]]
``` 