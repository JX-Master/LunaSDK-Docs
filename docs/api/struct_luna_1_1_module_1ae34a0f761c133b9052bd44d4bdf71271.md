# Luna::Module::get_name

```c++
virtual const c8 * get_name()=0
```

Gets one module name. Every module must have one unique name, and the name cannot changed after the module has been registered to the module system. 



## Return value
Returns one string that represents the module name. The lifetime of the string should be equal to the lifetime of the module. 

