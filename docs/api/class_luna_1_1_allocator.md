# Luna::Allocator
The default allocator implementation that can be used for allocating memory for containers defined in Runtime module. 

```c++
class Luna::Allocator
```

## Overview
The default allocator allocates memory by calling memalloc, and deallocates memory by calling memfree. 

## Functions
* [_Ty * allocate(usize n=1)](class_luna_1_1_allocator_1a8ed50dd7b8971bd8e18ed3a2d7dea9d1.md)

    Allocates memory for the specified number of elements. 

* [void deallocate(_Ty *ptr, usize n=1)](class_luna_1_1_allocator_1a36cada72231a020cb53784c2fadba635.md)

    Deallocates memory allocated from allocate. 

