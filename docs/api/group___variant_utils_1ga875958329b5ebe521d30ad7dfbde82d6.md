# Luna::VariantUtils::write_json

```c++
RV write_json(IStream *stream, const Variant &v, bool indent=true)
```

Writes one variant object to JSON string. 



## Parameters
* *in* **stream**

    The stream to write JSON string to. 

* *in* **v**

    The variant object that contains data to write. 

* *in* **indent**

    Whether to add indents and line breaks to the generated JSON string, so that improves readability but also increases the string size. 

