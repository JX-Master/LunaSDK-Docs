# Luna::reset_flags

```c++
template <typename _Ty>
constexpr auto reset_flags(_Ty &flags, _Ty options) -> enable_if_t< is_enum_v< _Ty >, void >
```

Resets the provided enumeration options to 0. 

## Overview


## Parameters
### flags
The flag variable to reset. 

### options
The options to set to 0. 

