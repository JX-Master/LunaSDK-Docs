# Luna::Quaternion::operator/=

```c++
Quaternion & operator/=(const Quaternion &q)
```

Concatenates one inversed quaternion of `q` to this quaternions, and stores the result to this quaternion. 

This function performs the following operations: 
```
[Quaternion](struct_luna_1_1_quaternion_1aa6b3a49c0418a7fff323e09d0ec6c3b9.md) inv = [inverse](group___runtime_math_1gab0d9795335706f43984e0252900baa4e.md)(q);
*this = *this * inv;
```


## Parameters
* *in* **q**

    The quaternion to divide. 

## Return value
Returns `*this`. 

