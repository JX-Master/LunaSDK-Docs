# Luna::impl_interface_for_type

```c++
template <typename _Ty, typename _Ity1, typename...>
void impl_interface_for_type()
```

Registers one or more interface implementations for one type. 

## Remark
To register one or multiple interfaces for one type in one call, use the template version of `impl_interface_for_type` like so: [Interface](struct_luna_1_1_interface.md) should not be included when using `impl_interface_for_type`. The template version of `impl_interface_for_type` calls the non-template version automatically, so it will be more convenient than calling the non-template version directly. 

