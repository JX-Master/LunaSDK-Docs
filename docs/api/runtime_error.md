# Error handling
## Types
* [Luna::ErrCode](struct_luna_1_1_err_code.md)

    The error code type represents one single error. 


* [Luna::Error](struct_luna_1_1_error.md)

    The error object encapsulates one error code along with one string that describes the error. 


* [Luna::R](struct_luna_1_1_r.md)

    A wrapper object for the return value of one function that may fail. 


* [Luna::R< void >](struct_luna_1_1_r_3_01void_01_4.md)

    Specification of [R](struct_luna_1_1_r.md) for void type. 


## Alias types
* [using errcat_t =  usize](group___runtime_error_1ga2fb0ec3bd79226d7a6357732e810b3d9.md)

    The error category type represents one container that can hold multiple error codes and sub-categories. 

* [using RV =  R<void>](group___runtime_error_1gab6ff284901ba6c715fed0c96f8ee5c74.md)

    An alias of `R<void>` for representing one throwable function with no return value. 

## Constants
* [constexpr RV ok](group___runtime_error_1ga5b239ee8917aacd639e36743f8561eb2.md)

    A special constant result object that represents one successful result. You can return `ok` instead of `RV()` to clearly represent one successful call for one function without return value. 

## Functions
* [ErrCode get_error_code_by_name(const c8 *errcat_name, const c8 *errcode_name)](group___runtime_error_1gac2cf4135d372c8b93bc5dd51a1a5a3a2.md)

    Gets the error code represented by the error name. 

* [errcat_t get_error_category_by_name(const c8 *errcat_name)](group___runtime_error_1gac7e9fd4f2431ea0709d0899cfee536c7.md)

    Gets the error category represented by the error category name. 

* [const c8 * get_error_code_name(ErrCode err_code)](group___runtime_error_1ga75d9ae8fc66e253da7bc9d90167baaf0.md)

    Fetches the name of the error code. 

* [const c8 * get_error_category_name(errcat_t err_category)](group___runtime_error_1gadda3f4a1becfdbaf57a9fed96030f95b.md)

    Fetches the name of the error category. 

* [errcat_t get_error_code_category(ErrCode err_code)](group___runtime_error_1gaf28bcde18fe38cf58195e662ebcd8b4b.md)

    Fetches the error category that holds the error code. 

* [Vector< errcat_t > get_all_error_categories()](group___runtime_error_1gae082bb725c117dca8ebb6d4930a85148.md)

    Fetches all error categories registered in the system, including all subcategories. 

* [Vector< ErrCode > get_all_error_codes_of_category(errcat_t err_category)](group___runtime_error_1ga98bcabdee045687efff56c4ce5649e43.md)

    Fetches all error codes that belongs to the specified error category. 

* [Vector< errcat_t > get_all_error_subcategories_of_category(errcat_t err_category)](group___runtime_error_1ga3316dfabb9dec565b522b52d687313a9.md)

    Fetches all child error categories that belongs to the specified error category. 

* [Error & get_error()](group___runtime_error_1ga89d49593e13c02ae38a8d75c9700756c.md)

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

## Macros
* [lupanic_if_failed(_res)](group___runtime_error_1gac1a979c01037533b5f7ec07c635a41d6.md)

    Crashes the program if the specified result is failed. 

* [lupanic_if_failed_msg(_res, _msg)](group___runtime_error_1gaeb3e75ee53288d8bdf7fcac3889f22e7.md)

    Crashes the program if the specified result is failed with custom message. 

* [luerr](group___runtime_error_1ga24ac080adf09c45becbe0255f4e7c968.md)

    The error code used in `lucatch` block to identify the error. 

* [lutry](group___runtime_error_1ga27044b65837c4ae8ea0a267dd4b13670.md)

    Opens one try block that encapsulates expressions that may fail. 

* [luthrow(_r)](group___runtime_error_1ga6e2423aec58cef0861156156c0845805.md)

    Throws one error and jumps execution to the `lucatch` block. 

* [lucatch](group___runtime_error_1ga92d64054822274f5341a06e22ed519ee.md)

    Opens one catch block that handles errors thrown from try block. 

* [lucatchret](group___runtime_error_1ga52994675a8f990d3166434e361971324.md)

    Defines one catch block that returns the error code (if any) thrown from try block. 

* [luexp(_exp)](group___runtime_error_1ga618a04348c5eec9062aa85bae5fff91a.md)

    Tests whether the specified expression returns one failed result, and throws the error code if failed. 

* [luset(_v, _exp)](group___runtime_error_1gad360047f2ac9303c32e17ef565d83627.md)

    Assigns the return value of the specified expression to the specified variable if the return value is valid, and throws the error code if not. 

* [lulet(_v, _exp)](group___runtime_error_1ga1c5f015bbf7bd9d53e7b0cc6a4338142.md)

    Creates one local variable to hold the return value of the specified expression if the return value is valid, and throws the error code if not. 

