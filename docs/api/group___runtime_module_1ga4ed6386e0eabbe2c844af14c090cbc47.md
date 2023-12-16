# Luna::init_module

```c++
RV init_module(const Name &module_name)
```

Initializes the specified module and all dependency modules of the specified module. 



## Parameters
* *in* **module_name**

    The name of the specified module. 

## Remark
If the specified module is already initialized, this function does nothing and succeeds. 

