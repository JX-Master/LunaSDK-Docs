# Luna::Variant::insert

```c++
void insert(usize i, const Variant &val)
```

Copy-inserts one variant to the specified index. 



## Parameters
* *in* **i**

    The index to insert the variant to. 

* *in* **val**

    The variant to insert. 

## Valid Usage
* The current variant must be an array variant or a null variant. If the current variant is a null variant, it will be converted to an empty array variant before the insertion is performed.

* `i` must be smaller to equal to [size](class_luna_1_1_variant_1a79348f1b7c06b34052b42656a0279429.md). 

