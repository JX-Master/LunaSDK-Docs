# Luna::UniquePtr::UniquePtr

```c++
UniquePtr(pointer p)
```

Constructs one smart pointer by wrapping pointer `p`. 

The smart pointer will have unique ownership to `p`, and the pointer should not be owned by another smart pointer. 

## Parameters
* **p**

    The pointer to wrap. 

