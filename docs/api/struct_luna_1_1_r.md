# Luna::R
A wrapper object for the return value of one function that may fail. 

```c++
template <typename _Ty>
struct Luna::R
```

If the function succeeds, this object contains the return value; if the function fails, this object contains the error code so that it can be identified. 

