# Luna::VariantUtils::read_xml

```c++
R< Variant > read_xml(IStream *stream)
```

Parses one XML string. 



## Parameters
* *in* **stream**

    The stream that contains the XML string to read. [IStream::read](struct_luna_1_1_i_stream_1a6a5956c629eb0bba95dc0dd89bd0abde.md) will be called to read XML string from the stream. 

## Return value
Returns one variant that contains the data read from the XML string. 

