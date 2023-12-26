# Luna::is_over_aligned
Checks if the specified type's alignment requirement is greater than alignof(max_align_t). 

```c++
template <typename _Ty>
struct Luna::is_over_aligned : public non-virtual std::integral_constant< bool, impl::is_over_aligned< _Ty >()>
```

## Base type
* std::integral_constant< bool, impl::is_over_aligned< _Ty >()>
