# Luna::bit_test

```c++
bool bit_test(const void *base_addr, usize bit_offset)
```

Tests if specified bit is 1. 



## Parameters
* *in* **base_addr**

    The address of the bit to offset from. 

* *in* **bit_offset**

    The number of bits shifted from the `base_addr`. 

## Return value
Returns `true` if the bit is 1, `false` if the bit is 0. 

## Remark
The following cases demonstrate the index order of `bit_test`, `bit_set` and `bit_reset`.


base_addr: 0x1000, bit_offset: 0, `*((u8*)0x1000)`: 0000 1000b* test result: false.

* value of `*((u8*)0x1000)` after set: 0000 1001b

* value of `*((u8*)0x1000)` after reset: 0000 1000b.

base_addr: 0x1000, bit_offset: 3, `*((u8*)0x1000)`: 0000 1000b* test result: true.

* value of `*((u8*)0x1000)` after set: 0000 1000b

* value of `*((u8*)0x1000)` after reset: 0000 0000b.

base_addr: 0x1000, bit_offset: 8, `*((u8*)0x1001)`: 0000 1000b* test result: false.

* value of `*((u8*)0x1001)` after set: 0000 1001b

* value of `*((u8*)0x1001)` after reset: 0000 1000b.

base_addr: 0x1000, bit_offset: 11, `*((u8*)0x1001)`: 0000 1000b* test result: true.

* value of `*((u8*)0x1001)` after set: 0000 1000b

* value of `*((u8*)0x1001)` after reset: 0000 0000b. 

