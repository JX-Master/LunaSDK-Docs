# Luna::get_enum_options

```c++
Span< const EnumerationOptionDesc > get_enum_options(typeinfo_t type)
```

Gets options of the specified enumeration. 



## Parameters
### type
The type to query. 

## Return value
Returns options of the specified enumeration. The returned buffer is valid until SDK shutdown. Returns one empty range if `type` is not an enumeration type. 

## Valid Usage
* `type` must specify one valid type object. 

