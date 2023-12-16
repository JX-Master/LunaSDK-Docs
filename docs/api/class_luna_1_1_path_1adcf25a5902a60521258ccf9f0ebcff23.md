# Luna::Path::encode

```c++
String encode(PathSeparator separator=PathSeparator::slash, bool has_root=true) const
```

Encodes the current path to a string. 



## Parameters
* *in* **separator**

    The separator format to use. Default is slash since it is well supported by all major platforms. 

* *in* **has_root**

    Whether to add root name to the path string. 

## Return value
Returns the encoded path string. 

