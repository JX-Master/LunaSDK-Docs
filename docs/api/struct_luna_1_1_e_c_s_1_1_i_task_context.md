# Luna::ECS::ITaskContext
Used by task to read and write world data. 

```c++
struct Luna::ECS::ITaskContext : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual void begin(IWorld *world, TaskExecutionMode exec_mode, Span< typeinfo_t > read_components, Span< typeinfo_t > write_components)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a70083b518f41249adbeee9ac726945d1.md)

    Resets the task context and begins a new task. 

* [virtual IWorld * get_world()=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1ab0c7eb1cb31db9c2e654d178cd2bfed7.md)

    Gets the world which this task context is attached to. 

* [virtual R< EntityAddress > get_entity(entity_id_t id)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a60e5c0e7e8425639ed4b0ae361b84603.md)

    Gets the entity address for the specified entity. 

* [virtual entity_id_t add_entity()=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a4362ec44389b677ff8ffb051297e54d7.md)

    Adds one entity to the world. 

* [virtual void remove_entity(entity_id_t id)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1af854242392cee3c7678d1d0f8a0db160.md)

    Removes the specified entity from the world. 

* [virtual void remove_all_entities()=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1abe6064c6799e1ff52c466378ee3ee73d.md)

    Removes all entities in the world. 

* [virtual void set_target_entity(entity_id_t id)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a69cb7645f322bff6525b68cc0fb36fc1.md)

    Changes the target entity for succeeding component and tag modification calls, including: 

* [virtual void * add_component(typeinfo_t component_type, bool allow_overwrite=false, usize *data_index=nullptr)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a7bed9fc89853cd411c2b17e298414a17.md)

    Adds one component to the target entity. 

* [virtual void * get_temp_component_data(typeinfo_t component_type, usize index)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1ae49e20b4f7993d5472503ac3c8eb35dd.md)

    Gets the component data being added by `add_component`. 

* [virtual void remove_component(typeinfo_t component_type)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a1043ff82ef3d849a77d2bc73e02f9a57.md)

    Removes the specified component. 

* [virtual void remove_all_components()=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a22331b5e68e9bff15d25e6b3aab3cb73.md)

    Removes all components of the target entity. 

* [virtual void add_tag(entity_id_t tag)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a0c2acafb1dc8a61e1c7da0c28c1dae5b.md)

    Adds one tag to the target entity. Tags are entity ids that is used to group and filter entities. 

* [virtual void remove_tag(entity_id_t tag)=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a713cb5c7cc3df4d329c98ab87c76847f.md)

    Removes one id from the target entity. 

* [virtual void remove_all_tags()=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1a418c69b81b6589e97fba33979b2bf596.md)

    Removes all ids of the target entity. 

* [virtual void end()=0](struct_luna_1_1_e_c_s_1_1_i_task_context_1aa540e86022c1f72380d1014d98f38f43.md)

    Finishes the current task and lets succeeding tasks to be run. 

