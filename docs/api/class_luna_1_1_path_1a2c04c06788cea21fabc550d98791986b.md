# Luna::Path::equal_to

```c++
bool equal_to(const Path &rhs, PathComponent compared_components=PathComponent::all) const
```

Compares two paths for equality. 



## Parameters
* *in* **rhs**

    The path to compare with. 

* *in* **compared_components**

    The components to compare, default is to compare all components and only `true` if all components of both paths are equal. 

## Return value
Returns `true` if all compared components in both paths are equal. Returns `false` otherwise. 

