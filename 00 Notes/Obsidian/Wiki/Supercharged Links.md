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
Source:: [Supercharged Links](obsidian://show-plugin?id=supercharged-links-obsidian)
Related To::
***
# Body:
Modifies Links color, Emojis and background based on metadata and tags

# Configuration
Target Attribute for styling  `type, sub-type, color`

# Backup
.obsidian\plugins\supercharged-links-obsidian\Data.jason

![[Supercharged Links Backup.json]]
## V3.0
```
{
  "targetAttributes": [
    "type",
    "sub-type",
    "color"
  ],
  "targetTags": true,
  "getFromInlineField": true,
  "enableTabHeader": true,
  "activateSnippet": true,
  "enableEditor": true,
  "enableFileList": true,
  "enableBacklinks": true,
  "enableQuickSwitcher": true,
  "enableSuggestor": true,
  "selectors": [
    {
      "type": "tag",
      "name": "Status",
      "value": "MOC/1",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "495f-d2a0",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "tag",
      "name": "Status",
      "value": "MOC/2",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "1353-12e6",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "tag",
      "name": "Status",
      "value": "MOC/3",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "8f0a-6764",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "tag",
      "name": "Status",
      "value": "MOC/4",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "0a50-1858",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "tag",
      "name": "Status",
      "value": "MOC/5",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "8a5e-7807",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "tag",
      "name": "Status",
      "value": "Moc/6",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "e923-78a5",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "sub-Type",
      "value": "Video",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "59a7-8d8c",
      "selectText": false,
      "selectAppend": false,
      "selectPrepend": true,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "sub-Type",
      "value": "Idea",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "9630-e603",
      "selectText": false,
      "selectAppend": false,
      "selectPrepend": true,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "sub-Type",
      "value": "Tool",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "313f-b37d",
      "selectText": false,
      "selectAppend": false,
      "selectPrepend": true,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "sub-Type",
      "value": "To Revise",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "12fc-dbdc",
      "selectText": false,
      "selectAppend": false,
      "selectPrepend": true,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "sub-Type",
      "value": "Key",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "4cdf-9a90",
      "selectText": false,
      "selectAppend": false,
      "selectPrepend": true,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Red",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "eb73-e7b3",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Orange",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "a34d-403b",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Yellow",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "532a-edfd",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Green",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "bfe3-f2ed",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Blue",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "249b-4724",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Purple",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "cbb1-720e",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Pink",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "bee7-0118",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Brown",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "cc7b-82b0",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "type",
      "value": "Grey",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "f5ae-b583",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "color",
      "value": "Black",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "5575-2e32",
      "selectText": true,
      "selectAppend": false,
      "selectPrepend": false,
      "selectBackground": false
    },
    {
      "type": "attribute",
      "name": "sub-type",
      "value": "link",
      "matchCaseSensitive": false,
      "match": "exact",
      "uid": "0822-46b3",
      "selectText": false,
      "selectAppend": false,
      "selectPrepend": true,
      "selectBackground": false
    }
  ]
}
```



# Foot
```meta-bind-embed
[[Foot note]]
``` 