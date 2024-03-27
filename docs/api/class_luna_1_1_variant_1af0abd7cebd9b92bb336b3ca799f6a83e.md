# Luna::Variant::blob_detach

```c++
Blob blob_detach()
```

Detaches and gets the data of one BLOB variant as a [Blob](class_luna_1_1_blob.md) object. 

After this operation, this variant is still a BLOB variant, but contains no binary data ( [blob_data](class_luna_1_1_variant_1a97bb1d2166a90fcc5244e5d86c80b9be.md) returns `nullptr`, and [blob_size](class_luna_1_1_variant_1a3e5b168557975c0111113042905dc6fd.md) returns `0`). 

## Return value
Returns the detached blob data if the variant is a BLOB variant. Returns one empty [Blob](class_luna_1_1_blob.md) object otherwise. 

