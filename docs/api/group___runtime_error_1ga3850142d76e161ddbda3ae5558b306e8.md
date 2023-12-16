# Luna::R::operator=

```c++
R & operator=(R &&rhs)
```

Assigns the result object by moving from another result object. 

The return value will be move-assigned if valid. 

## Parameters
* *in* **rhs**

    The object to move from. 

## Return value
Returns `*this`. 

