# Luna::List::assign

```c++
template <typename _InputIt>
auto assign(_InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, void >
```

Replaces elements of the list by elements specified by one range. Elements in the range will be copy-inserted into the list. 



## Parameters
### first
The iterator pointing to the first element of the range. 

### last
The iterator pointing to the one-past-last element of the range. 

