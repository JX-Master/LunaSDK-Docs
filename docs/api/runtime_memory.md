# Memory allocation and deallocation
## Functions
* [LUNA_RUNTIME_API void * memalloc(usize size, usize alignment=0)](group___runtime_memory_1ga76969916b035a432b54deb6920d3259c.md)

    Allocates heap memory. 

* [LUNA_RUNTIME_API void memfree(void *ptr, usize alignment=0)](group___runtime_memory_1ga4bc8f37f2fe8c9100a8af16de794e3de.md)

    Frees heap memory. 

* [LUNA_RUNTIME_API void * memrealloc(void *ptr, usize size, usize alignment=0)](group___runtime_memory_1ga60e9e4772655c0a60fbd5e311010b6d5.md)

    Reallocates heap memory. 

* [LUNA_RUNTIME_API usize memsize(void *ptr, usize alignment=0)](group___runtime_memory_1ga49d8171ef4af8fbe6bbb6e4e6f82d69b.md)

    Gets the allocated size of one memory block. 

* [_Ty * memnew(_Args &&... args)](group___runtime_memory_1ga81e30b31f5e8a02f54478a634015e720.md)

    Allocates heap memory for one object and constructs the object. 

* [void memdelete(_Ty *o)](group___runtime_memory_1gaf95818ee40a0536baee3f539b019df5d.md)

    Destructs one object and frees its memory. 

