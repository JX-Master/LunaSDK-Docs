# Luna::ECS::ITaskContext::add_component

```c++
virtual void * add_component(typeinfo_t component_type, bool allow_overwrite=false, usize *data_index=nullptr)=0
```

Adds one component to the target entity. 



## Parameters
* *in* **component_type**

    The type of the component to add. 

* *in* **allow_overwrite**

    If this is `true` and the specified component already exists, this call overwrites the old data with the new data. If this is `false` and the specified component already exists, this call does nothing. 

* *out* **data_index**

    If specified, returns the data index which can be used to query data pointer at a future time. 

## Return value
Returns the pointer to the new component data. The pointer is valid until another component add call is issued on the same change list. The returned component data is uninitialized, it is user's responsibility to initialize the component data before committing this change list. The system does not track the component state, committing uninitialized component may result in undefined hehavior. 

