# Debugging
## Classes
* [Luna::ProfilerEvent](struct_luna_1_1_profiler_event.md)
* [Luna::ProfilerEventData::MemoryAllocate](struct_luna_1_1_profiler_event_data_1_1_memory_allocate.md)
* [Luna::ProfilerEventData::MemoryDeallocate](struct_luna_1_1_profiler_event_data_1_1_memory_deallocate.md)
* [Luna::ProfilerEventData::SetMemoryName](struct_luna_1_1_profiler_event_data_1_1_set_memory_name.md)
* [Luna::ProfilerEventData::SetMemoryType](struct_luna_1_1_profiler_event_data_1_1_set_memory_type.md)
* [Luna::ProfilerEventData::SetMemoryDomain](struct_luna_1_1_profiler_event_data_1_1_set_memory_domain.md)
## Functions
* [LUNA_RUNTIME_API void * allocate_profiler_event_data(usize size, usize alignment, void(*dtor)(void *)=nullptr)](group___runtime_profiler_1ga0c06788b2e5c93818d402bae7a237aa6.md)

    Allocates one temporary buffer that can be used to store event data for the next profiler event. 

* [void profiler_event_data_dtor(void *data)](group___runtime_profiler_1gaacde50ed0a5efd0e07c4cbb079ee9cf0.md)

    One helper function that calls the destructor of the specified type on the pointer. 

* [_Ty * allocate_profiler_event_data()](group___runtime_profiler_1gaef867b156feb1c7ad417885ee9bc0a76.md)

    Allocates one temporary object that can be used to store event data for the next profiler event. 

* [LUNA_RUNTIME_API void submit_profiler_event(u64 event_id)](group___runtime_profiler_1gac1c18a61488c579ee7e57689a00066f6.md)

    Submits one profiler event. 

* [LUNA_RUNTIME_API usize register_profiler_callback(const Function< on_profiler_event_t > &handler)](group___runtime_profiler_1ga0cbbf2ad299628457df57c5ab086d1b5.md)

    Registers one profiler callback function. 

* [LUNA_RUNTIME_API void unregister_profiler_callback(usize handler_id)](group___runtime_profiler_1ga96c6c6b48e4693f93f9a032c8e8bf24d.md)

    Unregisters one profiler callback function. 

* [LUNA_RUNTIME_API void memory_profiler_allocate(void *ptr, usize size)](group___runtime_profiler_1ga4f66b7d3d7446ab9831db2b85650fed9.md)

    Emits one PROFILER_EVENT_ID_MEMORY_ALLOCATE profiler event. 

* [LUNA_RUNTIME_API void memory_profiler_deallocate(void *ptr)](group___runtime_profiler_1ga484ebdca3d68138f5bf05b13bc2e67c9.md)

    Emits one PROFILER_EVENT_ID_MEMORY_DEALLOCATE profiler event. 

* [LUNA_RUNTIME_API void memory_profiler_set_memory_name(void *ptr, const c8 *name, usize str_size=USIZE_MAX)](group___runtime_profiler_1ga70a0f39db69fda4df489d3f375665d1c.md)

    Sets a debug name for the memory block, for example, the name of the resource file this memory block is allocated for. This function emits one PROFILER_EVENT_ID_SET_MEMORY_NAME profiler event. 

* [LUNA_RUNTIME_API void memory_profiler_set_memory_type(void *ptr, const c8 *type, usize str_size=USIZE_MAX)](group___runtime_profiler_1gae66e344319da2dbb8550975d289d5d08.md)

    Sets the type of the object this memory block. 

* [LUNA_RUNTIME_API void memory_profiler_set_memory_domain(void *ptr, const c8 *domain, usize str_size=USIZE_MAX)](group___runtime_profiler_1ga48f319dc9914aa2adce844ea385d28f5.md)

    Sets the memory domain. 

