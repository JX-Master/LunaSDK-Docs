# Luna::UniquePtr
A smart pointer that wraps one dynamically created object, and deletes the object when the pointer is destructed. 

```c++
template <typename _Ty, typename _Deleter>
class Luna::UniquePtr
```



## Parameters
* **_Ty**

    The type of the object to wrap. 

* **_Deleter**

    The object deletion function to use. 

## Member functions
* [constexpr UniquePtr()](class_luna_1_1_unique_ptr_1ac83d6339a667b6d1a8d40ee3f6925479.md)

    Constructs one null smart pointer. 

* [constexpr UniquePtr(nullptr_t)](class_luna_1_1_unique_ptr_1af9585499282f6e8d6133800d1edd6186.md)

    Constructs one null smart pointer with `nullptr_t`. 

* [UniquePtr(pointer p)](class_luna_1_1_unique_ptr_1a415d11e7ffae129716eaff4144fe28ba.md)

    Constructs one smart pointer by wrapping pointer `p`. 

* [UniquePtr(pointer p, const deleter_type &d)](class_luna_1_1_unique_ptr_1a13bbbabafab0a33a3a53569f45615d2c.md)

    Constructs one smart pointer by wrapping pointer `p` with custom object deletion function. 

* [UniquePtr(pointer p, deleter_type &&d)](class_luna_1_1_unique_ptr_1a054c4486b447589097e0224c71ed22f2.md)

    Constructs one smart pointer by wrapping pointer `p` with custom object deletion function. 

* [pointer get() const](class_luna_1_1_unique_ptr_1ae35ff781593cc93da0ce2fb918fff312.md)

    Gets the underlying native pointer. 

* [deleter_type & get_deleter()](class_luna_1_1_unique_ptr_1a05e7557ba281dac6ccaa4c36f618df54.md)

    Get the object deletion function. 

* [const deleter_type & get_deleter() const](class_luna_1_1_unique_ptr_1ac153c6620599410f50b4a4f367489c27.md)

    Get the object deletion function. 

* [operator bool() const](class_luna_1_1_unique_ptr_1a67b76affb3b5d35fa419ac234144038b.md)

    Checks whether this smart pointer is not null. 

* [add_lvalue_reference< _Ty >::type operator*() const](class_luna_1_1_unique_ptr_1a07b4045405c743defdaa0e5c82f9efca.md)

    Dereferences the native pointer. 

* [pointer operator->() const](class_luna_1_1_unique_ptr_1aef4e7d4e0fa56e9f7509c555f73d24d2.md)

    Accesses members of the instance pointed by the pointer. 

* [pointer release()](class_luna_1_1_unique_ptr_1a091d6047345ff0bce4545d27b0c8a97e.md)

    Sets the native pointer to null, and gets the original pointer. 

* [void reset(pointer ptr=pointer())](class_luna_1_1_unique_ptr_1a5216dc341de1b239241863a818bf0cbf.md)

    Sets the native pointer of this smart pointer. If this smart pointer is not null, the original instance pointed by this smart pointer will be deleted. 

* [void swap(UniquePtr &rhs)](class_luna_1_1_unique_ptr_1a45fea58c778fa56bba791b54bd20dbe2.md)

    Swaps native pointers of this smart pointer with the specified smart pointer. 

* [UniquePtr(UniquePtr &&rhs)](class_luna_1_1_unique_ptr_1a343f6b000e4d4c7a053445c3ba69f0f1.md)

    Constructs one smart pointer by moving native pointer from another smart pointer. 

* [UniquePtr & operator=(UniquePtr &&rhs)](class_luna_1_1_unique_ptr_1ad0257cfd9a6dda5785bee1162088d8a9.md)

    Assigns one smart pointer by moving native pointer from another smart pointer. If this smart pointer is not null, the original instance pointed by this smart pointer will be deleted. 

* [UniquePtr & operator=(nullptr_t)](class_luna_1_1_unique_ptr_1a876d8711a35f8b24b1e43fcccf13d6a5.md)

    Sets one smart pointer to null. If this smart pointer is not null, the original instance pointed by this smart pointer will be deleted. 

* [bool operator==(const UniquePtr &rhs) const](class_luna_1_1_unique_ptr_1ad2831fccce70add1eb456e93fd679f0a.md)

    Compares two smart pointers for equality. Two smart pointers are equal if their native pointers are equal or both null. 

* [bool operator!=(const UniquePtr &rhs) const](class_luna_1_1_unique_ptr_1acafa2825dfa07009c36fe4208f0a8203.md)

    Compares two smart pointers for non-equality. 

