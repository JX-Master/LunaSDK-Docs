# Luna::set_serializable

```c++
void set_serializable(typeinfo_t type, SerializableTypeDesc *desc=nullptr)
```

Sets one type to be serializable. 

## Parameters
* *in* **type**

    The type to set. 

* *in* **desc**

    The user-provided serialize and deserialize callback. If `nullptr` is specified, the system try to serialize the type bying serializing every property of the type. `nullptr` can only be specified if this is a structure type and all properties of this type is serializable. 

