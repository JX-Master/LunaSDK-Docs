# Luna::copy_if

```c++
template <typename _InputIt, typename _OutputIt, typename UnaryPredicate>
_OutputIt copy_if(_InputIt first, _InputIt last, _OutputIt d_first, UnaryPredicate pred)
```

Copies elements that pass user-defined function from one range to another range. The relative order of elements that are copied is preserved. 



## Parameters
* *in* **first**

    The iterator to the first element of the source range. 

* *in* **last**

    The iterator to the one-past-last element of the source range. 

* *in* **d_first**

    The iterator to the first element of the destination range. 

* *in* **pred**

    The user-defined unary predicate which returns `​true` for elements that should be copied. 

## Return value
Returns one iterator to the one-past-last element of the destination range. 

## Valid Usage
* The expression `pred(v)` must be convertible to `bool` for every argument `v` of type `VT`, where `VT` is the value type of `_InputIt`, and must not modify `v`. 

