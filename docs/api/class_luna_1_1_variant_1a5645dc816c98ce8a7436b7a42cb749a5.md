# Luna::Variant::blob_data

```c++
const byte_t * blob_data() const
```

Gets the data pointer of one BLOB variant. 



## Return value
Returns the data pointer if the variant is a BLOB variant with [blob_size](class_luna_1_1_variant_1a3e5b168557975c0111113042905dc6fd.md) greater than `0`. Returns `nullptr` otherwise. 

