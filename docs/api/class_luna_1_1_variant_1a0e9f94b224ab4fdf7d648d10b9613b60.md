# Luna::Variant::operator=

```c++
Variant & operator=(const Blob &blob_data)
```

Assigns one variant with one blob. The variant type will be [VariantType::blob](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233aee26908bf9629eeb4b37dac350f4754a.md) after this assignment. 



## Parameters
* *in* **blob_data**

    The blob data to set. The blob data will be copied into the variant. 

## Return value
Returns `*this`. 

