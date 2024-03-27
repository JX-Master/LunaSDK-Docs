# Luna::VariantUtils::write_xml

```c++
RV write_xml(IStream *stream, const Variant &v, bool indent=true)
```

Writes one variant object to XML string. 



## Parameters
* *in* **stream**

    The stream to write XML string to. 

* *in* **v**

    The variant object that represents the root XML element to write. 

* *in* **indent**

    Whether to add indents and line breaks to the generated XML string, so that improves readability but also increases the string size. 

