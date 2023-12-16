# Luna::register_struct_type

```c++
template <typename _Ty>
typeinfo_t register_struct_type(Span< const StructurePropertyDesc > properties, typeinfo_t base_type=nullptr)
```

Registers one structure type to the type system. The structure type must have one lustruct macro defined in the structure body. 



## Parameters
* *in* **properties**

    A list of properties that should be tracked by the type system. The user can use luproperty macro to declare properties conveniently. 

* *in* **base_type**

    The base type of the type to register. This can be `nullptr`. 

## Return value
Returns the registered structure type. 

