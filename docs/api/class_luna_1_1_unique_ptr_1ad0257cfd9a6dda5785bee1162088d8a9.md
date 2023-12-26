# Luna::UniquePtr::operator=

```c++
UniquePtr & operator=(UniquePtr &&rhs)
```

Assigns one smart pointer by moving native pointer from another smart pointer. If this smart pointer is not null, the original instance pointed by this smart pointer will be deleted. 



## Parameters
* *in* **rhs**

    The smart pointer to move pointer from. This smart pointer will be null after this operation. 

