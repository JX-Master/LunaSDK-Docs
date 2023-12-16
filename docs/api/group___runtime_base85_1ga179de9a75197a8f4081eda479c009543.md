# Luna::base85_get_encoded_size

```c++
constexpr usize base85_get_encoded_size(usize raw_size)
```

Get the encoded base85 string size from the raw data size. 



## Parameters
* *in* **raw_size**

    The size of the raw binary data in bytes. This size must be times of 4. 

## Return value
The size of the encoded string in bytes. The string size does not include the null-terminator. 

