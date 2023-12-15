# Luna::copy_relocate

```c++
template <typename _Iter1, typename _Iter2>
auto copy_relocate(_Iter1 dst, _Iter2 src) -> enable_if_t< Impl::copy_relocate_is_value_type_trivial< _Iter1, _Iter2 >::value, _Iter1 >
```

Relocates one object. 

After this call, the object in the destination memory behaves the same as the object formerly in the source memory, except that the place(memory address) for the object is changed. 

## Parameters
### dst
An iterator to relocation destination. 

### src
An iterator to the object to be relocated. 

## Return value
Returns `dst`. 

