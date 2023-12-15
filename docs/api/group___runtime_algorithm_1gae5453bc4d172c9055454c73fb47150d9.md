# Luna::find_if

```c++
template <typename _InputIt, typename _UnaryPredicate>
constexpr _InputIt find_if(_InputIt first, _InputIt last, _UnaryPredicate p)
```

Searches for the first element in the range that passes the user-provided unary predicate. 



## Parameters
### first
The iterator pointing to the first element of the search range. 

### last
The iterator pointing to the one-past-last element of the search range. 

### p
The user-provided unary predicate which will be called to test elements. 

## Return value
Returns one iterator pointing to the first element that `p(v)` is `true`. Returns `last` if not found. 

#### Valid Usage
* The expression `p(v)` must be convertible to `bool` for every argument `v` of type `VT`, where `VT` is the value type of `_InputIt`, and must not modify `v`. 

