# Luna::Variant::insert

```c++
bool insert(const Name &k, const Variant &val)
```

Copy-inserts the variant with the specified key as the child variant of the current variant. 



## Parameters
* *in* **k**

    The key string of the variant to insert. 

* *in* **val**

    The variant to insert. 

## Return value
Returns `true` if the variant is successfully inserted. Returns `false` if one variant with the specified key already exists, in such case, the existing variant is not modified. 

## Valid Usage
* The current variant must be an object variant or a null variant. If the current variant is a null variant, it will be converted to an empty object variant before the insertion is performed. 

