# Luna::set_equatable

```c++
void set_equatable(typeinfo_t type, equal_to_func_t *func)
```

Sets one type to support equality testing. 



## Parameters
* *in* **type**

    The type object. 

* *in* **func**

    The equality testing function to use. 

## Valid Usage
* `type` must specify one valid type object and cannot be a generic structure type.

* `func` must specify one valid function. 

