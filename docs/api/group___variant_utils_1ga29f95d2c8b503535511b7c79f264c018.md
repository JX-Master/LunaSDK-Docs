# Luna::VariantUtils::find_first_xml_child_element

```c++
const Variant & find_first_xml_child_element(const Variant &xml_element, const Name &name, usize start_index=0, usize *out_index=nullptr)
```

Finds the first XML child element in the specified XML element with the specified name. 



## Parameters
* *in* **xml_element**

    The variant that represents the parent XML element. 

* *in* **name**

    The name of the XML child element to search for. 

* *in* **start_index**

    The index to start searching for the specified element. 

* *out* **out_index**

    If not `nullptr`, returns the index of the found element. If the element is not found, returns [USIZE_MAX](group___runtime_base_type_1gaf70b42c748a1e2bec2022ea52a74954a.md). 

## Return value
Returns one reference to the found child element. Returns Variant::npos if not found. 

