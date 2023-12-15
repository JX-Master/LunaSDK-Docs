# Luna::errcat_t

```c++
using errcat_t =  usize
```

The error category type represents one container that can hold multiple error codes and sub-categories. 

## Overview
Like the error code, the category value will be determined when the error category is firstly accessed, and will never be changed.

Any valid error type number will not be 0. 

