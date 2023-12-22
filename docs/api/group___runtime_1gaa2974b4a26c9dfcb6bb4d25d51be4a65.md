# Luna::get

```c++
template <usize, typename...>
TupleElement< _I, Tuple< _Tys... > >::type const  & get(const Tuple< _Tys... > &t)
```

Gets the `_I`th element from the tuple. 



## Parameters
* *in* **t**

    The tuple to extract element from. 

## Return value
Returns one lvalue constant reference to the element in the tuple. 

