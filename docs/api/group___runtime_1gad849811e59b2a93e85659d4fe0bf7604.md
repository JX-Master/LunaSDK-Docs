# Luna::get

```c++
template <usize, typename...>
TupleElement< _I, Tuple< _Tys... > >::type volatile && get(volatile Tuple< _Tys... > &&t)
```

Gets the `_I`th element from the tuple. 



## Parameters
* *in* **t**

    The tuple to extract element from. 

## Return value
Returns one rvalue volatile reference to the element in the tuple. 

