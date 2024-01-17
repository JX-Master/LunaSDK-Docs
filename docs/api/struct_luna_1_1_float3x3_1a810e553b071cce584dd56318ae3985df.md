# Luna::Float3x3::data

```c++
f32 * data()
```

Gets the data of the matrix as one array of [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) elements. 

Note that the matrix is 16 bytes aligned, so the row pitch in array data is 16 bytes, or 4 elements. For example, to fetch the element at row 1 column 2, use `data()[4 * 1 + 2]`. 

## Return value
Returns one pointer to the data array. 

