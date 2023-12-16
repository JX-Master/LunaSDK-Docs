# Luna::register_boxed_type

```c++
template <typename _Ty>
typeinfo_t register_boxed_type()
```

Registers one type so that it can be used for creating boxed objects. 

This function only registers basic information for one type, it does not register properties, constructors and other information. Use [register_struct_type](group___runtime_type_1gabdbbe8b5d92239b0af155d9d04b78f1c.md) if you want a type with full reflection info. 

