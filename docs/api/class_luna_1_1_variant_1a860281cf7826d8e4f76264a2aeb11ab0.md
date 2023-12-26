# Luna::Variant::fnum

```c++
f64 fnum(f64 default_value=0) const
```

Gets the data of one number variant as one 64-bit floating-point number. 



## Parameters
* *in* **default_value**

    The optional default number to return. 

## Return value
Returns the value as one 64-bit floating-point number. If the value is in another number format, it will be converted automatically. Returns `default_value` if the variant is not a number variant. 

