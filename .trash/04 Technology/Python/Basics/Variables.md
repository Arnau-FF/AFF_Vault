# `= this.file.link`
>[!Properties]- | `= this.Parent.Parent.Parent.Parent` |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` |`BUTTON[note]` 
>Version:: 2.1
>Parent:: [[Basics]]
>Tags: #Notes
```meta-bind-embed
[[Search note]]
```
Source::
Related To::
***
#### To Consider:
- Variables are case sensitive. ➔ recommended to be lower case
- Can not contain spaces.

##  Boolean
```
is_published = False
is_published = True
```
True and False are *Case Sensitive* not Equal to true / false or TRUE / FALSE

##  Integer
```
cnv_speed = 1000
```

##  Floating Point
```
rating = 4.99
```

## String

```
recipe_name = "Ghost Mode"
recipe_name = 'Ghost Mode' # Also valid
```
- Line Break
```
# Option 1
string_line_break = """
This String
Has several
Line Breaks
"""
#Option 2
string_line_break = "This String \nHas several\nLine Breaks"  #\n = line break
```

- Array From String
```
name = "ABCDEFG"
name[0]   # A (index 0)
name[1]   # B (index 1)
name[-1]  # G (loops back, last character)
name[0:3] # ABC ( Firts 3 characters, last(3) not included.
```
String starts at index 0

- Scaped Character ➔ When a invalid character is part of a String ➔ (') (") 
```
name = "ABC"DEF" # ABC"DEF is an invalid String

#option 1
name = 'ABC"DEF'

#option 2
name = "ABC\"DEF" # \ Scapes charcter(").\Does not print.
``` 

## Lists

```
list [1,3,5,7,9]
```
# Foot
```meta-bind-embed
[[Foot note]]
``` 