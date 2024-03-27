# Luna::VariantUtils::patch

```c++
void patch(Variant &before, const Variant &delta)
```

Applys the difference to the variant, so that it contains the same data as `after` when the diff object is created. 



## Parameters
* *in* **before**

    The variant to patch. 

* *in* **delta**

    The delta variant returned by [diff](group___variant_utils_1gad66978526bf62fd780e0696831c786e3.md). 

## Return value
Returns the patched variant object. 

