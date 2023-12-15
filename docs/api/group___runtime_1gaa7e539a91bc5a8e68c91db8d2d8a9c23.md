# Luna::new_object

```c++
template <typename _Ty, typename...>
Ref< _Ty > new_object(_Args &&... args)
```

Creates one new boxed object. 

This function uses object_alloc to allocate one new boxed object, then use placement new operator to initialize the object. 

## Parameters
### args
The arguments to construct the new boxed object. 

## Return value
Returns one strong reference to the new boxed object. 

