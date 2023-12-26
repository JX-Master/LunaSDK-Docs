# Luna::Variant::inum

```c++
i64 inum(i64 default_value=0) const
```

Gets the data of one number variant as one signed 64-bit integer. 



## Parameters
* *in* **default_value**

    The optional default number to return. 

## Return value
Returns the value as one signed 64-bit integer. If the value is in another number format, it will be converted automatically. Returns `default_value` if the variant is not a number variant. 

