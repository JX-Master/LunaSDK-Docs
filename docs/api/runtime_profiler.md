# Debugging
## Types
* [Luna::ProfilerEvent](struct_luna_1_1_profiler_event.md)

    A emitted profiler event. 


* [Luna::ProfilerEventData::MemoryAllocate](struct_luna_1_1_profiler_event_data_1_1_memory_allocate.md)

    The memory allocation event data. 


* [Luna::ProfilerEventData::MemoryDeallocate](struct_luna_1_1_profiler_event_data_1_1_memory_deallocate.md)

    The memory deallocation event data. 


* [Luna::ProfilerEventData::SetMemoryName](struct_luna_1_1_profiler_event_data_1_1_set_memory_name.md)

    The set memory name event data. 


* [Luna::ProfilerEventData::SetMemoryType](struct_luna_1_1_profiler_event_data_1_1_set_memory_type.md)

    The set memory type event data. 


* [Luna::ProfilerEventData::SetMemoryDomain](struct_luna_1_1_profiler_event_data_1_1_set_memory_domain.md)

    The set memory domain event data. 


## Functions
* [void * allocate_profiler_event_data(usize size, usize alignment, void(*dtor)(void *)=nullptr)](group___runtime_profiler_1ga7eaa2c6dab0d6b10da8f589ae1faceaf.md)

    Allocates one temporary buffer that can be used to store event data for the next profiler event. 

* [void profiler_event_data_dtor(void *data)](group___runtime_profiler_1gaacde50ed0a5efd0e07c4cbb079ee9cf0.md)

    One helper function that calls the destructor of the specified type on the pointer. 

* [_Ty * allocate_profiler_event_data()](group___runtime_profiler_1gaef867b156feb1c7ad417885ee9bc0a76.md)

    Allocates one temporary object that can be used to store event data for the next profiler event. 

* [void submit_profiler_event(u64 event_id)](group___runtime_profiler_1ga9606e89a2918c82f675423172519de00.md)

    Submits one profiler event. 

* [usize register_profiler_callback(const Function< on_profiler_event_t > &handler)](group___runtime_profiler_1ga22959c4b1b3b648ea696bb268c925f32.md)

    Registers one profiler callback function. 

* [void unregister_profiler_callback(usize handler_id)](group___runtime_profiler_1ga61119861f9b1baaa12126748287a6a61.md)

    Unregisters one profiler callback function. 

* [void memory_profiler_allocate(void *ptr, usize size)](group___runtime_profiler_1ga93eae32928d521552eb67865e576c03d.md)

    Emits one PROFILER_EVENT_ID_MEMORY_ALLOCATE profiler event. 

* [void memory_profiler_deallocate(void *ptr)](group___runtime_profiler_1ga78750728333548e6d934696710eb64a5.md)

    Emits one PROFILER_EVENT_ID_MEMORY_DEALLOCATE profiler event. 

* [void memory_profiler_set_memory_name(void *ptr, const c8 *name, usize str_size=USIZE_MAX)](group___runtime_profiler_1ga731879fecbe041bf54b3a17f471ae93b.md)

    Sets a debug name for the memory block, for example, the name of the resource file this memory block is allocated for. This function emits one PROFILER_EVENT_ID_SET_MEMORY_NAME profiler event. 

* [void memory_profiler_set_memory_type(void *ptr, const c8 *type, usize str_size=USIZE_MAX)](group___runtime_profiler_1ga528082599fe26fa41bc437284edba5a6.md)

    Sets the type of the object this memory block. 

* [void memory_profiler_set_memory_domain(void *ptr, const c8 *domain, usize str_size=USIZE_MAX)](group___runtime_profiler_1ga29e87893674b7781230d72457b42d2db.md)

    Sets the memory domain. 

