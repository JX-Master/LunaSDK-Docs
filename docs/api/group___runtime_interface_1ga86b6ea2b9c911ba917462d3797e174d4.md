# Luna::query_interface

```c++
void * query_interface(object_t object, const Guid &iid)
```

Gets one interface pointer from one pointer to one boxed object that implements the interface. 



## Parameters
* *in* **object**

    The pointer to the boxed object to query interface from. 

* *in* **iid**

    The interface GUID to query. 

## Return value
Returns one pointer that can be safely reinterpreted to the specified interface pointer. Returns `nullptr` if the specified interface is not implemented by the specified boxed object. 

