# Luna::typeof

```c++
template <typename _Ty>
typeinfo_t typeof()
```

Gets the type object of the specified type. 



## Return value
Returns the type object of the specified type. Returns `nullptr` if the type is not registered. 

## Remark
This function calls [typeof_t](struct_luna_1_1typeof__t.md) internally to get the type object of the specified type. 

