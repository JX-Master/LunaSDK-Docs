# Luna::test_flags

```c++
template <typename _Ty>
constexpr auto test_flags(_Ty flags, _Ty options) -> enable_if_t< is_enum_v< _Ty >, bool >
```

Tests if the provided enumeration contains the specified enumeration option. 



## Parameters
### flags
The flags to test. 

### options
A combination of flags to test. 

## Return value
Returns `true` if all flags in the `options` combination are set in `flags`, returns `false` otherwise. 

