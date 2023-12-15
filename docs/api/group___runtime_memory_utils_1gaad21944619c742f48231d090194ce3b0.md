# Luna::bit_set

```c++
void bit_set(void *addr, usize bit_offset, bool value)
```

Sets the specified bit to 1 if `value` is `true`, or to 0 if `value` is `false`. 



## Parameters
### base_addr
The address of the bit to offset from. 

### bit_offset
The number of bits shifted from the `base_addr`. 

### value
The value to set for the bit. 

