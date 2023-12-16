# Luna::new_object

```c++
template <typename _Ty, typename...>
Ref< _Ty > new_object(_Args &&... args)
```

Creates one new boxed object. 

This function uses [object_alloc](group___runtime_object_1gabbcaac45f20e9e4c322fb1db0376b641.md) to allocate one new boxed object, then use placement new operator to initialize the object. 

## Parameters
* *in* **args**

    The arguments to construct the new boxed object. 

## Return value
Returns one strong reference to the new boxed object. 

