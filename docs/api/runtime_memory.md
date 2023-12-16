# Memory allocation and deallocation
## Functions
* [void * memalloc(usize size, usize alignment=0)](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md)

    Allocates heap memory. 

* [void memfree(void *ptr, usize alignment=0)](group___runtime_memory_1ga102bf0df13784b9f636c555461862a14.md)

    Frees heap memory. 

* [void * memrealloc(void *ptr, usize size, usize alignment=0)](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md)

    Reallocates heap memory. 

* [usize memsize(void *ptr, usize alignment=0)](group___runtime_memory_1gaa0742c7fff949c5eb1cabb3edb7d0a92.md)

    Gets the allocated size of one memory block. 

* [_Ty * memnew(_Args &&... args)](group___runtime_memory_1ga81e30b31f5e8a02f54478a634015e720.md)

    Allocates heap memory for one object and constructs the object. 

* [void memdelete(_Ty *o)](group___runtime_memory_1gaf95818ee40a0536baee3f539b019df5d.md)

    Destructs one object and frees its memory. 

