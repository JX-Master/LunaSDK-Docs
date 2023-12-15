# Error handling
## Classes
* [Luna::ErrCode](struct_luna_1_1_err_code.md)
* [Luna::Error](struct_luna_1_1_error.md)
* [Luna::R](struct_luna_1_1_r.md)
* [Luna::R< void >](struct_luna_1_1_r_3_01void_01_4.md)
## Aliasing types
* [using errcat_t =  usize](group___runtime_error_1ga2fb0ec3bd79226d7a6357732e810b3d9.md)

    The error category type represents one container that can hold multiple error codes and sub-categories. 

* [using RV =  R<void>](group___runtime_error_1gab6ff284901ba6c715fed0c96f8ee5c74.md)

    An alias of `[R](struct_luna_1_1_r.md)<void>` for representing one throwable function with no return value. 

## Functions
* [LUNA_RUNTIME_API ErrCode get_error_code_by_name(const c8 *errcat_name, const c8 *errcode_name)](group___runtime_error_1ga1f70b7b7d6832c50eca9fcee754738e5.md)

    Gets the error code represented by the error name. 

* [LUNA_RUNTIME_API errcat_t get_error_category_by_name(const c8 *errcat_name)](group___runtime_error_1gafe222dee1f7cd3d2beb8e32604dddd71.md)

    Gets the error category represented by the error category name. 

* [LUNA_RUNTIME_API const c8 * get_error_code_name(ErrCode err_code)](group___runtime_error_1ga282ca73bbf2ecb824b31f111225f452a.md)

    Fetches the name of the error code. 

* [LUNA_RUNTIME_API const c8 * get_error_category_name(errcat_t err_category)](group___runtime_error_1gaae9e733615f31d34d2caacc345f5cfa4.md)

    Fetches the name of the error category. 

* [LUNA_RUNTIME_API errcat_t get_error_code_category(ErrCode err_code)](group___runtime_error_1ga2d688464e553307f8a2399935db72da3.md)

    Fetches the error category that holds the error code. 

* [LUNA_RUNTIME_API Vector< errcat_t > get_all_error_categories()](group___runtime_error_1ga67d5908c99b79c7154f6e1e6e342a72e.md)

    Fetches all error categories registered in the system, including all subcategories. 

* [LUNA_RUNTIME_API Vector< ErrCode > get_all_error_codes_of_category(errcat_t err_category)](group___runtime_error_1gae1aeb6bafa3695ea3c6e6dc1acea72ff.md)

    Fetches all error codes that belongs to the specified error category. 

* [LUNA_RUNTIME_API Vector< errcat_t > get_all_error_subcategories_of_category(errcat_t err_category)](group___runtime_error_1gafa7d509a05e3f4029e5976bbfd8631f1.md)

    Fetches all child error categories that belongs to the specified error category. 

* [LUNA_RUNTIME_API Error & get_error()](group___runtime_error_1gae92623cecc5f4224389fda59a2b46707.md)

    Gets the error object of this thread. Every thread will be assigned with one error object. 

* [ErrCode set_error(ErrCode code, const c8 *fmt, VarList args)](group___runtime_error_1ga85a2f3789aeea2a659a102d8399f26c3.md)

    Sets the error object of this thread. 

* [ErrCode set_error(ErrCode code, const c8 *fmt,...)](group___runtime_error_1gaab150f9ec3b047217f5c2d2131c54c77.md)

    Sets the error object of this thread. 

* [const c8 * explain(ErrCode err_code)](group___runtime_error_1gad578dbba7b4f8b2b7fa8bcd956a1efb0.md)

    Gets a brief description about the error code. 

* [ErrCode unwrap_errcode(ErrCode err_code)](group___runtime_error_1ga3f9510c74cc3eb31228045014ea1a07c.md)

    Gets the real error code if the error code is BasicError::error_object. 

* [bool valid() const](group___runtime_error_1ga315419f26d3c59fa143b49b90a019049.md)

    Tests if the result is successful and the return value is valid. 

* [R(const _Ty &v)](group___runtime_error_1gae270572a4f9d80793694a4686a2a0473.md)

    Constructs one successful result object with the specified return value. 

* [R(_Ty &&v)](group___runtime_error_1ga2a0b45d4070ca962d1dd9f7a0694e278.md)

    Constructs one successful result object with the specified return value. 

* [R(ErrCode error)](group___runtime_error_1gae6df6df63f7880dfb63cb8611239bab3.md)

    Constructs one failed result object with the specified error code. 

* [R(const R &rhs)](group___runtime_error_1gad72c3b57b3e6f30877c4d031b641fe68.md)

    Constructs one result object by coping from another result object. 

* [R(R &&rhs)](group___runtime_error_1ga630a7366db11b0fa684c26aa9736478b.md)

    Constructs one result object by moving from another result object. 

* [R & operator=(const R &rhs)](group___runtime_error_1ga3b25cc5b71c28d9d8a52f82cc688871f.md)

    Assigns the result object by coping from another result object. 

* [R & operator=(R &&rhs)](group___runtime_error_1ga3850142d76e161ddbda3ae5558b306e8.md)

    Assigns the result object by moving from another result object. 

* [const _Ty & get() const](group___runtime_error_1ga99f878496613323217993a6b57e6e7f6.md)

    Gets the return value of the result object. 

* [_Ty & get()](group___runtime_error_1ga38a9abd57df742d690f2ca0c668abab8.md)

    Gets the return value of the result object. 

* [ErrCode errcode() const](group___runtime_error_1gacaa89fc96cb4e21f5274b5a082fdde98.md)

    Gets the error code of the result object. 

* [bool valid() const](group___runtime_error_1ga315419f26d3c59fa143b49b90a019049.md)

    Tests if the result is successful. 

* [constexpr R()](group___runtime_error_1gae87adf00c177c791effe51865404096d.md)

    Constructs one successful result object. 

* [R(ErrCode error)](group___runtime_error_1gae6df6df63f7880dfb63cb8611239bab3.md)

    Constructs one failed result object with the specified error code. 

* [R(const R &rhs)](group___runtime_error_1gad72c3b57b3e6f30877c4d031b641fe68.md)

    Constructs one result object by coping from another result object. 

* [R & operator=(const R &rhs)](group___runtime_error_1ga3b25cc5b71c28d9d8a52f82cc688871f.md)

    Assigns the result object by coping from another result object. 

* [ErrCode errcode() const](group___runtime_error_1gacaa89fc96cb4e21f5274b5a082fdde98.md)

    Gets the error code of the result object. 

* [bool succeeded(const R< _Ty > &r)](group___runtime_error_1ga1fe2ca7a6a977e75b7922af899b927c9.md)

    Tests whether the specified result is successful. 

* [bool failed(const R< _Ty > &r)](group___runtime_error_1ga4c75c58a9d262021f330194d48d5acd2.md)

    Tests whether the specified result is failed. 

* [ErrCode unwrap_errcode(const R< _Ty > &obj)](group___runtime_error_1gad35f7f747a4f2cc86d549a67c090681a.md)

    Unwraps the real error code from the result. 

