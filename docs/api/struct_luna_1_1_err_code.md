# Luna::ErrCode
The error code type represents one single error. 

```c++
struct Luna::ErrCode
```

## Overview
In Luna Runtime, every error is represented by one error code, the code value will be determined when the error is firstly accessed, and will never be changed.

Any valid error code number will not be 0.

The error code is wrapped in a unique structure so that it will never be misinterpreted to a normal return value when the function return value is also an integer. 

## Properties
* [usize code](struct_luna_1_1_err_code_1a77ca0743e6dd02f1f1ca0b3f5a772388.md)

    The identifier of the error code. 

