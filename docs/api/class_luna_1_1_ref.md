# Luna::Ref
The smart pointer that represents one typed strong reference to one boxed object. 

```c++
template <typename _Ty>
class Luna::Ref
```

## Member functions
* [void reset()](class_luna_1_1_ref_1ad20897c5c8bd47f5d4005989bead0e55.md)

    Resets the reference to null. 

* [bool valid() const](class_luna_1_1_ref_1a315419f26d3c59fa143b49b90a019049.md)

    Checks whether this reference is valid. 

* [object_t object() const](class_luna_1_1_ref_1aa35fe176621b16279c1bde6c9f242af5.md)

    Gets the boxed object. 

* [_Ty * get() const](class_luna_1_1_ref_1a0c62005b5c43288845fcc6d3e177bd8b.md)

    Gets the boxed object casted to `_Ty`. 

* [_Ty * operator->() const](class_luna_1_1_ref_1afc2ad7a38eefaa297c20a07fa669a674.md)

    Gets the boxed object casted to `_Ty`. 

* [void attach(object_t ptr)](class_luna_1_1_ref_1a7be0b40dc76fc93f46c2ae9316513142.md)

    Attaches provided pointer. 

* [object_t detach()](class_luna_1_1_ref_1a8b980cb86bd65155f3240b3a00597e6c.md)

    Detaches the stored pointer. The reference becomes null after this operation. 

* [Ref()](class_luna_1_1_ref_1a8cb1ae7f0793df666b8a09f606e6ac44.md)

    Constructs one null reference. 

* [Ref(const Ref &rhs)](class_luna_1_1_ref_1af080798d5ee0c1c7e3714c9f1eef19c8.md)

    Constructs one reference by coping the pointer from another reference of the same type. 

* [Ref(Ref &&rhs)](class_luna_1_1_ref_1ab91bfef355bf234da318c997538097d9.md)

    Constructs one reference by moving the pointer from another reference of the same type. 

* [Ref & operator=(const Ref &rhs)](class_luna_1_1_ref_1abab12019678beb9e1714ec156e5a678c.md)

    Assigns this reference by coping the pointer from another reference of the same type. 

* [Ref & operator=(Ref &&rhs)](class_luna_1_1_ref_1a9ea7a476b6cca6ec37adf26e42eee6b0.md)

    Assigns this reference by moving the pointer from another reference of the same type. 

* [Ref(const Ref< _Rty > &rhs)](class_luna_1_1_ref_1af7d21b3f738d8731703c6378ba20ce77.md)

    Constructs one reference by coping the pointer from another reference of one different type. 

* [Ref & operator=(const Ref< _Rty > &rhs)](class_luna_1_1_ref_1a1dca4a71bb24c736f5a3b09263b2742e.md)

    Assigns this reference by coping the pointer from another reference of one different type. 

* [Ref(Ref< _Rty > &&rhs)](class_luna_1_1_ref_1a54a36e8f2a667d7f560dd031236ab682.md)

    Constructs one reference by moving the pointer from another reference of one different type. 

* [Ref & operator=(Ref< _Rty > &&rhs)](class_luna_1_1_ref_1a2db44e247ecbb0e6c05c590d5fa0818c.md)

    Assigns this reference by moving the pointer from another reference of one different type. 

* [Ref(_Ty *ptr)](class_luna_1_1_ref_1a532310075c287e3d05ad8ab7ab44b18c.md)

    Constructs one reference using the native pointer of the same type. 

* [Ref & operator=(_Ty *ptr)](class_luna_1_1_ref_1a2de641defb8a484bd1812d784e3af0e8.md)

    Assigns this reference using the native pointer of the same type. 

* [Ref(_Rty *ptr)](class_luna_1_1_ref_1a111a3aed594614582dba180a5b807e1d.md)

    Constructs one reference using the native pointer of one different type. 

* [Ref(const ObjRef &rhs)](class_luna_1_1_ref_1a726e3844670c9dd7c3f3a118a6bbe9a5.md)

    Constructs one reference by coping the pointer from one typeless reference. 

* [Ref(ObjRef &&rhs)](class_luna_1_1_ref_1aa7bb102b7487a97e50f3ce4cf40e2e3f.md)

    Constructs one reference by moving the pointer from one typeless reference. 

* [Ref & operator=(const ObjRef &rhs)](class_luna_1_1_ref_1a286e50de153d783006fcf2c3475f5ef8.md)

    Assigns this reference by coping the pointer from one typeless reference. 

* [Ref & operator=(ObjRef &&rhs)](class_luna_1_1_ref_1a883e3f228b14c8960e1ba648358388af.md)

    Assigns this reference by moving the pointer from one typeless reference. 

* [bool operator==(const Ref &rhs) const](class_luna_1_1_ref_1a523237139b59716450886f730457a30c.md)

    Compares two references for equality. 

* [bool operator!=(const Ref &rhs) const](class_luna_1_1_ref_1a5e55bfc932dd471834f05a1fcd192484.md)

    Compares two references for non-equality. 

* [bool operator==(_Ty *rhs) const](class_luna_1_1_ref_1ad918ea8b0e2ae19ad3abb31fc87f5559.md)

    Compares one reference with one native pointer for equality. 

* [bool operator!=(_Ty *rhs) const](class_luna_1_1_ref_1a5c8675c3964f3c1313663a72d9d1c7f1.md)

    Compares one reference with one native pointer for non-equality. 

* [bool operator<(const Ref &rhs) const](class_luna_1_1_ref_1a6b77fdc84e8c622c126fbc7c1e2b5f29.md)

    Compares two references. 

* [operator _Ty *() const](class_luna_1_1_ref_1aa137966a77920b6f8564c03bbe1bf5b2.md)

    Gets the boxed object casted to `_Ty`. 

* [_Rty * as() const](class_luna_1_1_ref_1a2a03b2d9c01bf054359744d25ba13be9.md)

    Gets the boxed object casted to `_Rty`. 

