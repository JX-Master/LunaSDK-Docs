# Luna::Allocator::deallocate

```c++
template <typename _Ty>
void deallocate(_Ty *ptr, usize n=1)
```

Deallocates memory allocated from [allocate](class_luna_1_1_allocator_1a8ed50dd7b8971bd8e18ed3a2d7dea9d1.md). 



## Parameters
* *in* **ptr**

    The memory pointer returned by [allocate](class_luna_1_1_allocator_1a8ed50dd7b8971bd8e18ed3a2d7dea9d1.md). 

* *in* **n**

    The number of elements earler passed to [allocate](class_luna_1_1_allocator_1a8ed50dd7b8971bd8e18ed3a2d7dea9d1.md). 

