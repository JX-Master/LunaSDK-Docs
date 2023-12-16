# Luna::memdelete

```c++
template <typename _Ty>
void memdelete(_Ty *o)
```

Destructs one object and frees its memory. 



## Parameters
* *in* **o**

    The pointer to the object to be deleted. 

## Valid Usage
* `o` must point to a object created by `memnew`. 

