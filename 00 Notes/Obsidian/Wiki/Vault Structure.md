---
Type: Note
---
# `= this.file.link`
>[!Properties]- |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]` 
>Version:: 3
>Parent:: [[Wiki]]
>Tags:
```meta-bind-embed
[[Search note]]
```
Source::
Related To::
***
# Structure
The structure is defined by the `Parent` field in each note’s metadata.  
Every note has a **parent**, except for the Dashboard, which sits at the top.

## Layout

Dashboard
├── Areas
│   ├── Themes
│   │   ├── Notes / Projects / Resources / Archive
│   │   │   └── (Child Notes — infinite depth)
└── Index (Sidebar)

### Dashboard 

- Top-level Map of Content (MOC Level 1)
- The parent of **all** notes
- Displays vault stats, structure, and high-level info
- Still a work in progress
### Areas
- Corresponds to Moc/2  (Map of Content Level2 )
- High-level categories like: `Work`, `Personal`, `Projects`, `Obsidian`, `Woodworking`.
- Can contain multiple Themes.
### Themes
- Corresponds to Moc/3  (Map of Content Level3 )
- A specific topic within an Area.
- Contains multiple Notes related to the theme.
### Notes
There are a series of Dropdown list to configure and modify some properties of the Note.
#### Type :
##### Notes
- One idea per note.
- Usually short and focused.
##### Projects
- Collections of related notes.
- Often tied to a goal or outcome.
##### Resources
- References, tools, external links.
- Support material for multiple notes or projects.
##### Archive
- Outdated or no longer active notes.
- Hidden from main views.

#### Sub-Type
Adds an emoji to the start of the note based on the sub-type selected.
It uses [[Supercharged Links]] and [[Style Settings]].
#### Color
Changes the link color.
It uses [[Supercharged Links]] and [[Style Settings]].
#### Priority
Helps to order notes on the search list based on the Priority value.
0 Priority  ➔ Top
9 Priority  ➔ Bottom

# Navigation

- Open any **Area** or **Theme** note directly from the **Index**, pinned to the left sidebar.
- Every note includes a **4-level deep visual hierarchy**, showing links to all its parent notes for easy context and navigation.




# Foot
```meta-bind-embed
[[Foot note]]
``` 