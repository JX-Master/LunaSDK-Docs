# Luna::nullptr_t

```c++
using nullptr_t =  std::nullptr_t
```

`usize` is the unsigned integer type of whose length marches the machine architecture. In particular, in 32-bit application, this is 32-bit unsigned integer; in 64-bit application, this is 64-bit unsigned integer. The `usize` type is guaranteed to be large enough to store a indexable memory address, so that any pointer can be reinterpreted casted to `usize`. `isize` is similar to `usize` , but is a signed integer type, so this can be used to store the result of subtracting two pointers, and can be used to offset memory addresses and pointers. 

