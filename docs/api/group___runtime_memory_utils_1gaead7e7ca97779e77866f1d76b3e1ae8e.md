# Luna::addressof

```c++
template <typename _Ty>
_Ty * addressof(_Ty &value)
```

Gets the real address for object or function `value`, even if the `operator&` of the object has been overloaded. 

## Overview


## Parameters
### value
The object to fetch address. 

## Return value
Returns one pointer to the object. 

