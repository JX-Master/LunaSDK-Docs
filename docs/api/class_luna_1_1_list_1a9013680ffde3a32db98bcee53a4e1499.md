# Luna::List::List

```c++
template <typename _InputIt>
List(enable_if_t<!is_integral_v< _InputIt >, _InputIt > first, _InputIt last, const allocator_type &alloc=allocator_type())
```

Constructs a list with elements specified by one range. Elements in the range will be copy-inserted into the list. 



## Parameters
### first
The iterator pointing to the first element of the range. 

### last
The iterator pointing to the one-past-last element of the range. 

### alloc
The allocator to use. The allocator object will be copy-constructed into the list. 

