# Luna::VariantUtils::read_xml

```c++
R< Variant > read_xml(const void *src, usize src_size=USIZE_MAX)
```

Parses one XML string. 



## Parameters
* *in* **src**

    The XML string to read. 

* *in* **src_size**

    The maximum number of characters to read in `src`. The actual read chacaters may be small than this if the XML string ends early.


If this value is greater than `strlen(src)`, `strlen(src)` will be used as the maximum number of characters to read instead of this value. So specifing [USIZE_MAX](group___runtime_base_type_1gaf70b42c748a1e2bec2022ea52a74954a.md) will let the system detects the string length automatically. 

## Return value
Returns one variant that contains the data read from the XML string. 

