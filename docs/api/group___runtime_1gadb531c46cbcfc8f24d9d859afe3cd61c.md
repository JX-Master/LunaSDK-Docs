# Luna::set_flags

```c++
template <typename _Ty>
constexpr auto set_flags(_Ty flags, _Ty options, bool value) -> enable_if_t< is_enum_v< _Ty >, _Ty >
```

Sets the provided enumeration options to 1 or 0 based on the value provided. 

## Overview


## Parameters
### flags
The original flags before set. 

### options
The options to set to 1 or 0. 

### value
If this is `true`, all options specified will be set to 1, else they will be set to 0. 

## Return value
Returns the enumeration after all options specified being set. 

