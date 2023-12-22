# Luna::Tuple::Tuple

```c++
template <typename _UTy1, typename...>
Tuple(const Tuple< _UTy1, _UTys... > &rhs)
```

Constructs one tuple by coping elements from another tuple. 

The element types of two tuples do not need to be equal, so long as every element in target tuple can be copy constructed from the corresponding element in source tuple. 

## Parameters
* *in* **rhs**

    The tuple to copy elements from. 

