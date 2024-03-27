# Luna::VariantUtils::write_json

```c++
String write_json(const Variant &v, bool indent=true)
```

Writes one variant object to JSON string. 



## Parameters
* *in* **v**

    The variant object that contains data to write. 

* *in* **indent**

    Whether to add indents and line breaks to the generated JSON string, so that improves readability but also increases the string size. 

## Return value
Returns the generated JSON string. 

