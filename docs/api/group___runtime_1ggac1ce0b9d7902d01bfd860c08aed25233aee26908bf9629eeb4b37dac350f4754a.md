# Luna::VariantType::blob

```c++
blob = 6
```

Indicates a BLOB (binary large object) variant. 

A BLOB variant can store arbitrary binary data. The data pointer, size and alignment of the data can be fetched by calling Variant::blob_data, Variant::blob_size and Variant::blob_alignment methods. 

