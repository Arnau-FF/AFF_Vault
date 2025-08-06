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
Source:: [Callout Manager](obsidian://show-plugin?id=callout-manager)
Related To::
***
# Body:
Edits callouts Style from obsidian no CSS needed.

# Backup
.obsidian\plugins\callout-manager\Data.json
![[Callout Manager Backup.json]]
## V3.0 
```
{
  "callouts": {
    "custom": [
      "properties",
      "notes",
      "project",
      "archive",
      "metadata",
      "mentioned",
      "children",
      "type",
      "habit",
      "resource"
    ],
    "settings": {
      "properties": [
        {
          "changes": {
            "icon": "lucide-list",
            "color": "219, 219, 219"
          }
        }
      ],
      "notes": [
        {
          "changes": {
            "icon": "lucide-sticky-note",
            "color": "60, 179, 113"
          }
        }
      ],
      "project": [
        {
          "changes": {
            "icon": "lucide-rocket",
            "color": "70, 130, 180"
          }
        }
      ],
      "archive": [
        {
          "changes": {
            "icon": "lucide-folders",
            "color": "219, 219, 219"
          }
        }
      ],
      "metadata": [
        {
          "changes": {
            "icon": "lucide-binary",
            "color": "219, 219, 219"
          }
        }
      ],
      "mentioned": [
        {
          "changes": {
            "icon": "lucide-milestone",
            "color": "155, 109, 255"
          }
        }
      ],
      "children": [
        {
          "changes": {
            "icon": "lucide-arrow-right-to-line",
            "color": "0, 184, 169"
          }
        }
      ],
      "type": [
        {
          "changes": {
            "icon": "lucide-bolt",
            "color": "219, 219, 219"
          }
        }
      ],
      "habit": [
        {
          "changes": {
            "icon": "lucide-check"
          }
        }
      ],
      "resource": [
        {
          "changes": {
            "icon": "lucide-wrench"
          }
        },
        {
          "condition": {
            "colorScheme": "light"
          },
          "changes": {
            "color": "255, 215, 0"
          }
        },
        {
          "condition": {
            "colorScheme": "dark"
          },
          "changes": {
            "color": "253, 215, 0"
          }
        }
      ]
    }
  },
  "calloutDetection": {
    "obsidian": true,
    "theme": true,
    "snippet": true
  }
}
```







# Foot
```meta-bind-embed
[[Foot note]]
``` 