# Luna::VariantUtils::revert

```c++
void revert(Variant &after, const Variant &delta)
```

Reverts the difference made in `after`, so that it contains the same data as `before` when the diff object is created. 



## Parameters
* *in* **after**

    The variant to revert. 

* *in* **delta**

    The delta variant returned by [diff](group___variant_utils_1gad66978526bf62fd780e0696831c786e3.md). 

## Return value
Returns the reverted variant object. 

