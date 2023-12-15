# Luna::query_interface

```c++
template <typename _Ity>
_Ity * query_interface(object_t object)
```

Gets one interface pointer from one pointer to one boxed object that implements the interface. 



## Parameters
### object
The pointer to the boxed object to query interface from. 

## Return value
Returns the specified interface pointer for the boxed object. Returns `nullptr` if the specified interface is not implemented by the specified boxed object. 

