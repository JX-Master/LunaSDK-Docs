# Luna::VariantUtils::write_xml

```c++
String write_xml(const Variant &v, bool indent=true)
```

Writes one variant object to XML string. 



## Parameters
* *in* **v**

    The variant object that represents the root XML element to write. 

* *in* **indent**

    Whether to add indents and line breaks to the generated XML string, so that improves readability but also increases the string size. 

## Return value
Returns the generated XML string. 

