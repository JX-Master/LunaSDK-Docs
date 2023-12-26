# Luna::Variant::at

```c++
const Variant & at(usize i) const
```

Gets the child variant when this is an array variant. 



## Parameters
* *in* **i**

    The index of the child variant to fetch. 

## Return value
Returns one reference to the child variant at the specified index. Returns npos if the current variant is not an array variant, or if the index is invalid. 

