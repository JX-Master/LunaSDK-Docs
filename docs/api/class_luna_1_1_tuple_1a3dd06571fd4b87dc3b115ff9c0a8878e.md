# Luna::Tuple::Tuple

```c++
template <typename _UTy1, typename...>
Tuple(_UTy1 &&arg1, _UTys &&... args)
```

Constructs one tuple with every element being converted from the specified value. 

Values are passed to the constructor of elements using forward. 

## Parameters
* *in* **arg1**

    The value used to initialize the first tuple element. 

* *in* **args**

    Values used to initialize the rest tuple elements. 

