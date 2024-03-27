# Luna::ECS::ITaskContext::remove_entity

```c++
virtual void remove_entity(entity_id_t id)=0
```

Removes the specified entity from the world. 



## Parameters
* *in* **id**

    The ID of the entity to remove. 

## Remark
If the entity does not exist when this operation is committed, this operation does nothing. 

