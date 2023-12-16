# Luna::get_library_function

```c++
R< void * > get_library_function(opaque_t handle, const c8 *symbol)
```

Gets the function address (function pointer) of one function in the library from its symbol name. 



## Parameters
* *in* **handle**

    The library handle returned by [load_library](group___runtime_d_l_l_1ga4047beea74e118348cddab00150eb4f8.md). 

* *in* **symbol**

    The function's symbol name. 

## Return value
Returns the function address of the specified function. 

