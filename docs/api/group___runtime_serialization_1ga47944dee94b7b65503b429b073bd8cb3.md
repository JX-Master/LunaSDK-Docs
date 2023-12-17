# Luna::set_serializable

```c++
template <typename _Ty>
void set_serializable(SerializableTypeDesc *desc=nullptr)
```

Sets one type `_Ty` to be serializable. 

## Parameters
* *in* **desc**

    The user-provided serialize and deserialize callback. If `nullptr` is specified, the system try to serialize the type bying serializing every property of the type. `nullptr` can only be specified if this is a structure type and all properties of this type is serializable. 

