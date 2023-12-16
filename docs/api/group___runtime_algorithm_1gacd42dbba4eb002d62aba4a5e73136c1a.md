# Luna::find_if_not

```c++
template <typename _InputIt, typename _UnaryPredicate>
constexpr _InputIt find_if_not(_InputIt first, _InputIt last, _UnaryPredicate q)
```

Searches for the first element in the range that fails the user-provided unary predicate. 



## Parameters
* *in* **first**

    The iterator pointing to the first element of the search range. 

* *in* **last**

    The iterator pointing to the one-past-last element of the search range. 

* *in* **q**

    The user-provided unary predicate which will be called to test elements. 

## Return value
Returns one iterator pointing to the first element that `q(v)` is `false`. Returns `last` if not found. 

## Valid Usage
* The expression `q(v)` must be convertible to `bool` for every argument `v` of type `VT`, where `VT` is the value type of `_InputIt`, and must not modify `v`. 

