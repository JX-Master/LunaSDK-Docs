# Luna::Tuple::Tuple

```c++
template <typename _UTy1, typename...>
Tuple(Tuple< _UTy1, _UTys... > &&rhs)
```

Constructs one tuple by moving elements from another tuple. 

The element types of two tuples do not need to be equal, so long as every element in target tuple can be move constructed from the corresponding element in source tuple. 

## Parameters
* *in* **rhs**

    The tuple to move elements from. 

