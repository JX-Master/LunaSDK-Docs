# Luna::Function< _R(_Args...)>::operator()

```c++
_R operator()(_Args... args) const
```

Invokes the function wrapper. This will invoke the callable object that is stored in the function. 



## Parameters
* *in* **args**

    The arguments passed to the callable object. 

## Return value
Returns the return value of the callable object if `_R` is not `void`. Returns nothing otherwise. 

