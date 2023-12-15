# Luna::all_of

```c++
template <typename _InputIt, typename _UnaryPredicate>
constexpr bool all_of(_InputIt first, _InputIt last, _UnaryPredicate p)
```

Checks if the unary predicate returns `true` for all elements in the range. 



## Parameters
### first
The iterator pointing to the first element of the range. 

### last
The iterator pointing to the one-past-last element of the range. 

### p
The user-provided unary predicate which will be called to test elements. 

## Return value
Returns `ture` if the unary predicate returns `true` for all elements in the range. Returns `false` otherwise. 

#### Valid Usage
* The expression `p(v)` must be convertible to `bool` for every argument `v` of type `VT`, where `VT` is the value type of `_InputIt`, and must not modify `v`. 

