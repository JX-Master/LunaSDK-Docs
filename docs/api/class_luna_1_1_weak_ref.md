# Luna::WeakRef
The smart pointer that represents one typed weak reference to one boxed object. 

```c++
class Luna::WeakRef
```

## Functions
* [void reset()](class_luna_1_1_weak_ref_1ad20897c5c8bd47f5d4005989bead0e55.md)

    Resets the reference to null. 

* [bool valid() const](class_luna_1_1_weak_ref_1a315419f26d3c59fa143b49b90a019049.md)

    Checks whether this reference is valid. 

* [object_t object() const](class_luna_1_1_weak_ref_1aa35fe176621b16279c1bde6c9f242af5.md)

    Gets the boxed object. 

* [WeakRef()](class_luna_1_1_weak_ref_1a931d441cb2ce42d1b99a4f27191f86f6.md)

    Constructs one null reference. 

* [WeakRef(const WeakRef &rhs)](class_luna_1_1_weak_ref_1a6aa90ee83e8f7fe220ce9206c4d53ef3.md)

    Constructs one reference by coping the pointer from another reference of the same type. 

* [WeakRef(WeakRef &&rhs)](class_luna_1_1_weak_ref_1a7f87b543b6961a11c59e71670e03633e.md)

    Constructs one reference by moving the pointer from another reference. 

* [WeakRef & operator=(const WeakRef &rhs)](class_luna_1_1_weak_ref_1a9f6be6ccd380471b4f72cac3553ecd24.md)

    Assigns this reference by coping the pointer from another reference of the same type. 

* [WeakRef & operator=(WeakRef &&rhs)](class_luna_1_1_weak_ref_1ab24b03c6da517e2d7a81783441fc0ce8.md)

    Assigns this reference by moving the pointer from another reference of the same type. 

* [WeakRef(const Ref< _Ty > &rhs)](class_luna_1_1_weak_ref_1a702244fb6dc28ced79f38c2f9f0a4448.md)

    Constructs one weak reference from one strong reference of the same type. 

* [WeakRef & operator=(const Ref< _Ty > &rhs)](class_luna_1_1_weak_ref_1ab65fb1011f2337038338956e8a0c75d4.md)

    Assigns this reference by coping the pointer from one strong reference of the same type. 

* [bool operator==(const WeakRef &rhs) const](class_luna_1_1_weak_ref_1a0e25e45b431942b3b6b3b3b264d4c423.md)

    Compares two references for equality. 

* [bool operator!=(const WeakRef &rhs) const](class_luna_1_1_weak_ref_1afb9da8b47f78ad237089422c75f65edf.md)

    Compares two references for non-equality. 

* [bool operator<(const WeakRef &rhs) const](class_luna_1_1_weak_ref_1a5f1661fef3e84060b69b0166f65b35ab.md)

    Compares two references. 

* [operator bool() const](class_luna_1_1_weak_ref_1a67b76affb3b5d35fa419ac234144038b.md)

    Checks whether this reference is valid. 

* [Ref< _Ty > pin() const](class_luna_1_1_weak_ref_1aaaf46c2b360fbb282e6d5704f02fb7e7.md)

    Creates one strong reference from this weak reference. 

