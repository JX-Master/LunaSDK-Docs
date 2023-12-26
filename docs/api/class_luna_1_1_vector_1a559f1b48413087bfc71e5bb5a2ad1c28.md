# Luna::Vector::operator=

```c++
Vector< _Ty, _Alloc > & operator=(Vector &&rhs)
```

Replaces elements of the vector by moving elements from another vector. 



## Parameters
* *in* **rhs**

    The vector to move elements from. This vector will be empty after this operation. 

## Return value
Returns `*this`. 

