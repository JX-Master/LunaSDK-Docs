# Luna::set_flags

```c++
template <typename _Ty>
constexpr auto set_flags(_Ty &flags, _Ty options) -> enable_if_t< is_enum_v< _Ty >, void >
```

Sets the provided enumeration options to 1. 



## Parameters
### flags
The flag variable to set. 

### options
The options to set to 1. 

