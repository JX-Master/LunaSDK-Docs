# Luna::ObjRef
The smart pointer that represents one typeless strong reference to one boxed object. 

```c++
class Luna::ObjRef
```

## Functions
* [void reset()](class_luna_1_1_obj_ref_1ad20897c5c8bd47f5d4005989bead0e55.md)

    Resets the reference to null. 

* [bool valid() const](class_luna_1_1_obj_ref_1a315419f26d3c59fa143b49b90a019049.md)

    Checks whether this reference is valid. 

* [object_t get() const](class_luna_1_1_obj_ref_1a1c56e321384fe3edf65345f272d774fc.md)

    Gets the boxed object. 

* [void attach(object_t ptr)](class_luna_1_1_obj_ref_1a7be0b40dc76fc93f46c2ae9316513142.md)

    Attaches provided pointer. 

* [object_t detach()](class_luna_1_1_obj_ref_1a8b980cb86bd65155f3240b3a00597e6c.md)

    Detaches the stored pointer. The reference becomes null after this operation. 

* [ObjRef()](class_luna_1_1_obj_ref_1a1ba3eb3ceae46d4bc4b6d09430ffd620.md)

    Constructs one null reference. 

* [ObjRef(const ObjRef &rhs)](class_luna_1_1_obj_ref_1a17c9fbece817be82a9e608789d97bd60.md)

    Constructs one reference by coping the pointer from another reference. 

* [ObjRef(ObjRef &&rhs)](class_luna_1_1_obj_ref_1ad1d6c7854b7bb70e4472870503b90fcd.md)

    Constructs one reference by moving the pointer from another reference. 

* [ObjRef & operator=(const ObjRef &rhs)](class_luna_1_1_obj_ref_1a41df0b6f925a2dae8825f304c1144cbf.md)

    Assigns this reference by coping the pointer from another reference. 

* [ObjRef & operator=(ObjRef &&rhs)](class_luna_1_1_obj_ref_1a493ad14c2b79b5f2331783f88d97c0b5.md)

    Assigns this reference by moving the pointer from another reference. 

* [ObjRef(object_t ptr)](class_luna_1_1_obj_ref_1a42f8a12dc6b3fb4c189af9ef37d2da0e.md)

    Constructs one reference by providing the underlying pointer directly. 

* [ObjRef & operator=(object_t rhs)](class_luna_1_1_obj_ref_1a0d4850ee757648dcfbe03ddafc2fd405.md)

    Replaces the underlying pointer of this reference with the given pointer. 

* [bool operator==(const ObjRef &rhs) const](class_luna_1_1_obj_ref_1ad8f4fdca727abf909c72d5ee3554790d.md)

    Compares two references for equality. 

* [bool operator!=(const ObjRef &rhs) const](class_luna_1_1_obj_ref_1a644c3ae10bfb0268fe3c29e353e0b55c.md)

    Compares two references for non-equality. 

* [bool operator<(const ObjRef &rhs) const](class_luna_1_1_obj_ref_1a11ee9c316d4e82ce3923aa5954852ccf.md)

    Compares two references. 

* [typeinfo_t type() const](class_luna_1_1_obj_ref_1a31d709143dcc4de3e30d4f7f56a13580.md)

    Gets the type object of the boxed object. 

* [operator bool() const](class_luna_1_1_obj_ref_1a67b76affb3b5d35fa419ac234144038b.md)

    Checks whether this reference is valid. 

