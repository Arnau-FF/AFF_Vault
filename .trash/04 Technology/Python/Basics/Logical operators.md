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
# AND:
```
income = True
credit =  True

if income and creit :
    print("ok")
else:
    print("NO OK")
```

# OR:
```
income = True
credit =  True

if income or creit :
    print("ok")
else:
    print("NO OK")
```

# NOT:

```
income = True
credit =  True
student = True

if  not student:
    print("ok")
else:
    print("NO OK")
```

# Combination
 - Add ()
```
income = True
credit =  True
student = True

if  (income or credit) and not student:
    print("ok")
else:
    print("NO OK")
```

# Foot
```meta-bind-embed
[[Foot note]]
``` 