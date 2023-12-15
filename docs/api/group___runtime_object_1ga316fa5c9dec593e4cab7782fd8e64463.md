# Luna::register_boxed_type

```c++
template <typename _Ty>
typeinfo_t register_boxed_type()
```

Registers one type so that it can be used for creating boxed objects. 

## Overview
This function only registers basic information for one type, it does not register properties, constructors and other information. Use register_struct_type if you want a type with full reflection info. 

