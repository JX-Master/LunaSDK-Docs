# Luna::IRandom
Represents a Pseudo-random number generator. 

```c++
interface Luna::IRandom : public virtual Interface
```

## Functions
* [virtual void set_seed(u32 seed)=0](struct_luna_1_1_i_random_1aea5e5d0ead35d611e22be97fef9d4ad0.md)

    Sets random seed for the generator. 

* [virtual u32 gen_u32()=0](struct_luna_1_1_i_random_1a4e97435ea0c68b5c755fbdc51dcfda81.md)

    Generates one random 32-bit unsigned integer. 

* [virtual i32 gen_i32()=0](struct_luna_1_1_i_random_1acdcf572b4cd6adebd10cf13f98d1c640.md)

    Generates one random 32-bit signed integer. 

* [virtual u64 gen_u64()=0](struct_luna_1_1_i_random_1a947974c4ce35f1f686128d421cc82246.md)

    Generates one random 64-bit unsigned integer. 

* [virtual i64 gen_i64()=0](struct_luna_1_1_i_random_1a7981e3767a4abf932de843d0eb7e06b2.md)

    Generates one random 64-bit signed integer. 

* [virtual f32 gen_f32(f32 range_begin, f32 range_end)=0](struct_luna_1_1_i_random_1adf32755ca3030b6b3bbcf8bb1df021ba.md)

    Generates one random 32-bit floating-point number. 

* [virtual f64 gen_f64(f64 range_begin, f64 range_end)=0](struct_luna_1_1_i_random_1a060934db2fb7c3013799f6fbef4a4231.md)

    Generates one random 64-bit floating-point number. 

* [virtual Guid gen_guid()=0](struct_luna_1_1_i_random_1ace8b125c8fda7da43adea042fafa1cf7.md)

    Generates one random GUID (Globally Unique Identifier). 

