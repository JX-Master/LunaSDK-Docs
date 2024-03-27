# Luna::VFS::register_driver

```c++
void register_driver(const Name &name, const DriverDesc &desc)
```

Registers one new VFS driver to the system. 



## Parameters
* *in* **name**

    The name of the driver. If one driver that has the same name already exists in the system, the old driver will be replaced by the new driver. 

* *in* **desc**

    The descriptor of the driver. 

