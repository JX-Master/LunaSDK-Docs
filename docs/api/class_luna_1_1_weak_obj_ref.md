# Luna::WeakObjRef
The smart pointer that represents one typeless weak reference to one boxed object. 

```c++
class Luna::WeakObjRef
```

## Functions
* [void reset()](class_luna_1_1_weak_obj_ref_1ad20897c5c8bd47f5d4005989bead0e55.md)

    Resets the reference to null. 

* [bool valid() const](class_luna_1_1_weak_obj_ref_1a315419f26d3c59fa143b49b90a019049.md)

    Checks whether this reference is valid. 

* [object_t get() const](class_luna_1_1_weak_obj_ref_1a1c56e321384fe3edf65345f272d774fc.md)

    Gets the boxed object. 

* [void attach(object_t ptr)](class_luna_1_1_weak_obj_ref_1a7be0b40dc76fc93f46c2ae9316513142.md)

    Attaches provided pointer. 

* [object_t detach()](class_luna_1_1_weak_obj_ref_1a8b980cb86bd65155f3240b3a00597e6c.md)

    Detaches the stored pointer. The reference becomes null after this operation. 

* [WeakObjRef()](class_luna_1_1_weak_obj_ref_1af5b8dbc0845b4ae06e0282238300cc88.md)

    Constructs one null reference. 

* [WeakObjRef(const WeakObjRef &rhs)](class_luna_1_1_weak_obj_ref_1a36466d5931b88276f96fb42bdcb5129c.md)

    Constructs one reference by coping the pointer from another reference. 

* [WeakObjRef(WeakObjRef &&rhs)](class_luna_1_1_weak_obj_ref_1ab364b38c62c8ab3f1d76767f6e233da0.md)

    Constructs one reference by moving the pointer from another reference. 

* [WeakObjRef & operator=(const WeakObjRef &rhs)](class_luna_1_1_weak_obj_ref_1aa33ac6a09f5c20c7c708544a9f914f09.md)

    Assigns this reference by coping the pointer from another reference. 

* [WeakObjRef & operator=(WeakObjRef &&rhs)](class_luna_1_1_weak_obj_ref_1a169c54555e3a8f25622ad3b332a5c660.md)

    Assigns this reference by moving the pointer from another reference. 

* [WeakObjRef(const ObjRef &rhs)](class_luna_1_1_weak_obj_ref_1aa26b6268bdd12d66947b7ae6c0c61028.md)

    Constructs one weak reference from one strong reference. 

* [WeakObjRef & operator=(const ObjRef &rhs)](class_luna_1_1_weak_obj_ref_1ae029dea2956d9779fadbcfa5c55927e3.md)

    Assigns this reference by coping the pointer from one strong reference. 

* [WeakObjRef(object_t rhs)](class_luna_1_1_weak_obj_ref_1a09577bca14140885ea414330cc9634ea.md)

    Constructs one reference by providing the underlying pointer directly. 

* [WeakObjRef & operator=(object_t rhs)](class_luna_1_1_weak_obj_ref_1a908ad4f960e681b49662883f689e8fb8.md)

    Replaces the underlying pointer of this reference with the given pointer. 

* [bool operator==(const WeakObjRef &rhs) const](class_luna_1_1_weak_obj_ref_1a8ae3a46cc5b5e10fa2c6b04818317413.md)

    Compares two references for equality. 

* [bool operator!=(const WeakObjRef &rhs) const](class_luna_1_1_weak_obj_ref_1a9e1e1a9d41c945724bf81587eda9b60d.md)

    Compares two references for non-equality. 

* [bool operator<(const WeakObjRef &rhs) const](class_luna_1_1_weak_obj_ref_1ad3714842385b187235170a18e5bd02f8.md)

    Compares two references. 

* [operator bool() const](class_luna_1_1_weak_obj_ref_1a67b76affb3b5d35fa419ac234144038b.md)

    Checks whether this reference is valid. 

* [ObjRef pin() const](class_luna_1_1_weak_obj_ref_1af6347ac675db0acd160d0b36e8418dfd.md)

    Creates one strong reference from this weak reference. 

