# Luna::Vector::data

```c++
Vector< _Ty, _Alloc >::pointer data()
```

Gets one pointer to the data buffer of this vector. 



## Return value
Returns one pointer to the data buffer of this vector. The returned pointer may be `nullptr` if `size()` is `0`, which indicates that the data buffer is not allocated yet. 

