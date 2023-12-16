# Luna::base85_get_decoded_size

```c++
constexpr usize base85_get_decoded_size(usize encoded_size)
```

Get the decoded binary size from the encoded base85 string size. 



## Parameters
* *in* **encoded_size**

    The size of the encoded string, in bytes, and not including the null terminator. The size of the string must be times of 5. 

## Return value
The size of the decoded raw data, in bytes. 

