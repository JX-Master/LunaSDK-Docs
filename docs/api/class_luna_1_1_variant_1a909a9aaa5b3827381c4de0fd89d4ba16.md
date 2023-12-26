# Luna::Variant::find

```c++
const Variant & find(const Name &k) const
```

Gets the child variant when this is an object variant. 



## Parameters
* *in* **k**

    The key string of the child variant to fetch. 

## Return value
Returns the child variant with the specified key. Returns npos if the current variant is not an object variant, or if the key is not found. 

