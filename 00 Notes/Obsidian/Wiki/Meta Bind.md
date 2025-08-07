---
Type: Note
---
# `= this.file.link`
>[!Properties]- |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]` 
>Version:: 3
>Parent:: [[Plugins]]
>Tags:
```meta-bind-embed
[[Search note]]
```
Source:: [Meta Bind](obsidian://show-plugin?id=obsidian-meta-bind-plugin)
Related To::
***
# Body:
Creates templates to apply to embed to all notes
Generates buttons and drop don list to modify metadata values.

# Configuration
`By Default`

## Button Templates
Activates the command created by templater attached to a template, 
Use the create command instead of the insert command.
### Areas (Moc2)
```
label: +
icon: ""
hidden: false
class: moc2
tooltip: ""
id: moc2
style: default
actions:
  - type: command
    command: templater-obsidian:09 Templates/Notes/MOC2/Template_MOC2.md

```
### Themes (Moc3)
```
label: +
icon: ""
hidden: false
class: moc3
tooltip: ""
id: moc3
style: default
actions:
  - type: command
    command: templater-obsidian:09 Templates/Notes/MOC3/Template_MOC3.md

```
### Notes
```
label: +
icon: ""
hidden: false
class: note
tooltip: ""
id: note
style: default
actions:
  - type: command
    command: templater-obsidian:09 Templates/Notes/New Note/Template_Note.md

```


# Foot
```meta-bind-embed
[[Foot note]]
``` 