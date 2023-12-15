# Luna::Function< _R(_Args...)>
A function wrapper that can store one callable object, and enable coping, moving and invoking of such callable object. 

```c++
struct Luna::Function< _R(_Args...)>
```

## Overview
The callable object can be a function pointer or a function object (types that overloads `operator()`). 

## Functions
* [Function()](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1aa61125691a5b694a46ce9f6a0fbe5093.md)

    Constructs an empty function wrapper. 

* [Function(nullptr_t)](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1a707a672fcfb2919f438281489a7569a6.md)

    Constructs an empty function wrapper with `nullptr`. 

* [Function(const Function &rhs)](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1aaa1331a0ab0a16714e13741cb222b448.md)

    Constructs an function wrapper by coping from another function object. 

* [Function(Function &&rhs)](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1adcbe3cde1f4efd2a3b309daf49335129.md)

    Constructs an function wrapper by moving from another function object. 

* [Function(function_t *func)](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1a1a29300c0dc1f7b4626742cf73e7fce4.md)

    Constructs an function wrapper using one function pointer. 

* [Function(_Ty &&value)](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1adc64cd4d9d95878073c69d08821b2ae9.md)

    Constructs an function wrapper using one function object. 

* [void swap(Function &rhs)](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1a02f45d9e3b871201d65c991313c54970.md)

    Swaps the data of this function wrapper with another function wrapper. 

* [bool empty() const](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Tests whether this function wrapper is empty. 

* [operator bool() const](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1a67b76affb3b5d35fa419ac234144038b.md)

    Tests whether this function wrapper is non-empty. 

* [_R operator()(_Args... args) const](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4_1a4461cffc0d61cfd185d3297e539d5f27.md)

    Invokes the function wrapper. This will invoke the callable object that is stored in the function. 

