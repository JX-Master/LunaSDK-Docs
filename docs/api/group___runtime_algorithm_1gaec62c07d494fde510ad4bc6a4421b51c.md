# Luna::for_each

```c++
template <typename _InputIt, typename _UnaryFunction>
constexpr _UnaryFunction for_each(_InputIt first, _InputIt last, _UnaryFunction f)
```

Applies the given function object to every element in the range, in order. 

## Overview


## Parameters
### first
The iterator pointing to the first element of the range. 

### last
The iterator pointing to the one-past-last element of the range. 

### f
The user-defined unary function object to be applied. 

## Return value
Returns `f`. 

#### Valid Usage
* `f` must have the following function signature: `void f(const Type& v)`, where `Type` is the value type of `_InputIt`. 

