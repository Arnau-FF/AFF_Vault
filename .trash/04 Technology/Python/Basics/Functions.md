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
# What is it?

Reusable code that does an specific task.

Can be Built-in or imported from a library.

Or hand made.

### Parameter Vs argument

Param is when defining a function, argument is the value of said parameter

## Structure

```
function_name(argument2,argument2)
```
Arguments can be variables or data?

## Definition
```
def function_name(parameter):
    print(argument)
```
## Return Value (output)
```
def function_name(parmeter):
    return parameter+1

  
value = function_name(1)
print(value)
```

## Key word Argument
makes code more understandable
```
def add(a, b):
    return a+b

  
value = add(1, b= 2) # b= is just for knowing the name of the second argument. 
print(value)

```

## Default Parameters
Optional parameters

First declare mandatory parameters, after optional
```
def add(a, b=1): # b = 1 by default if not given another value
    return a+b

  
value = add(1, b= 2) 
print(value)

```


# Foot
```meta-bind-embed
[[Foot note]]
``` 