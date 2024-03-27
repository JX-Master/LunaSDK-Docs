# Luna::ECS::ITaskContext::get_temp_component_data

```c++
virtual void * get_temp_component_data(typeinfo_t component_type, usize index)=0
```

Gets the component data being added by `add_component`. 



## Parameters
* *in* **component_type**

    The component type to get. 

* *in* **index**

    The index of the component fetched from `add_component`. 

## Return value
Returns the pointer to the component data. The pointer is valid until another component add call is issued on the same change list. 

