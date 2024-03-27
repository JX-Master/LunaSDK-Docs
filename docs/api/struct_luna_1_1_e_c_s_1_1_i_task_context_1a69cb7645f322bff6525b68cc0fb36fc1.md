# Luna::ECS::ITaskContext::set_target_entity

```c++
virtual void set_target_entity(entity_id_t id)=0
```

Changes the target entity for succeeding component and tag modification calls, including: 

* `add_component`

* `remove_component`

* `set_component`

* `remove_all_components`

* `add_tag`

* `remove_tag`

* `remove_all_tags`

