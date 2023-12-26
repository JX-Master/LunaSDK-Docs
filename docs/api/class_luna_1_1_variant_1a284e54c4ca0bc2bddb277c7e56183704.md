# Luna::Variant::at

```c++
Variant & at(usize i)
```

Gets the child variant when this is an array variant. 



## Parameters
* *in* **i**

    The index of the child variant to fetch. 

## Return value
Returns one reference to the child variant at the specified index. 

## Valid Usage
* The current variant must be an array variant.

* `i` must be smaller than [size](class_luna_1_1_variant_1a79348f1b7c06b34052b42656a0279429.md) of the variant. 

