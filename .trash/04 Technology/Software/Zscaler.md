# `= this.file.link`
>[!Properties]- | `= this.Parent.Parent.Parent.Parent` |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` |`BUTTON[note]` 
>Version:: 2.1
>Parent:: [[00 Notes/04 Technology/Software/Software]]
>Tags: #Notes
```meta-bind-embed
[[Search note]]
```
Source::
Related To::
***
# Deactivate Zscaler:
## Power shell ➔ admin
### Status
```
Get-NetAdapterBinding -AllBindings -ComponentID ZS_ZAPPRD
```
### Disable
```
Get-NetAdapterBinding -AllBindings -ComponentID ZS_ZAPPRD | Disable-NetAdapterBinding
```
### Enable

```
Get-NetAdapterBinding -AllBindings -ComponentID ZS_ZAPPRD | Enable-NetAdapterBinding
```









# Foot
```meta-bind-embed
[[Foot note]]
``` 