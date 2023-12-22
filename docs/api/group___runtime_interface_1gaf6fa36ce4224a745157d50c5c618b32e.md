# Luna::query_interface

```c++
template <typename _Ity>
_Ity * query_interface(object_t object)
```

Gets one interface pointer from one pointer to one boxed object that implements the interface. 



## Parameters
* *in* **object**

    The pointer to the boxed object to query interface from. 

## Return value
Returns the specified interface pointer for the boxed object. Returns `nullptr` if the specified interface is not implemented by the specified boxed object. 

## Remark
The template version of `query_interface` provides a more convenient way to fetch one interface pointer from one boxed object pointer like so: 
```
[object_t](group___runtime_object_1ga4d287a1c3bd0821c2391f4613686e35a.md) object = ...;
Interface1* i = query_interface<Interface1>(object);
```


