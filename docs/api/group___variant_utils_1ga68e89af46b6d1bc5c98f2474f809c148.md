# Luna::VariantUtils::read_json

```c++
R< Variant > read_json(IStream *stream)
```

Parses one JSON string. 



## Parameters
* *in* **stream**

    The stream that contains the JSON string to read. [IStream::read](struct_luna_1_1_i_stream_1a6a5956c629eb0bba95dc0dd89bd0abde.md) will be called to read JSON string from the stream. 

## Return value
Returns one variant that contains the data read from the JSON string. 

