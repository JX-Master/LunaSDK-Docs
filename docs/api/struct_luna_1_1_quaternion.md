# Luna::Quaternion
Used to represent one rotation operaiton using four [f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) values. 

```c++
struct Luna::Quaternion
```

## Member objects
* [f32 x](struct_luna_1_1_quaternion_1a6b05cac69c0301ab972c27ce208373be.md)

    The fist component of the quaternion. 

* [f32 y](struct_luna_1_1_quaternion_1ab7291adeb8828a0cba3aedf332c2053d.md)

    The second component of the quaternion. 

* [f32 z](struct_luna_1_1_quaternion_1aac280fcf3516d20b5e3dec5fa770ac50.md)

    The third component of the quaternion. 

* [f32 w](struct_luna_1_1_quaternion_1adb390a9d0e1ce3b726f016e547104e35.md)

    The fourth component of the quaternion. 

* [f32 m[4]](struct_luna_1_1_quaternion_1a913c09d0cc2a1dab1ceb500fd8704174.md)

    The array of components. 

## Member functions
* [Quaternion()=default](struct_luna_1_1_quaternion_1aa6b3a49c0418a7fff323e09d0ec6c3b9.md)

    Constructs one quaternion with components uninitialized. 

* [Quaternion(const Quaternion &)=default](struct_luna_1_1_quaternion_1a61ed587fd2173523275e04740f45af78.md)

    Constructs one quaternion by coping components from another quaternion. 

* [Quaternion & operator=(const Quaternion &)=default](struct_luna_1_1_quaternion_1ac47f0f2db69004986b02c528547edbfc.md)

    Assigns one quaternion by coping components from another quaternion. 

* [Quaternion(Quaternion &&)=default](struct_luna_1_1_quaternion_1acc08fcc8e8fac90a89a3b12c25d8737b.md)

    Constructs one quaternion by coping components from another quaternion. 

* [Quaternion & operator=(Quaternion &&)=default](struct_luna_1_1_quaternion_1a490986dd899e623a77d058655e568957.md)

    Assigns one quaternion by coping components from another quaternion. 

* [constexpr Quaternion(f32 x, f32 y, f32 z, f32 w)](struct_luna_1_1_quaternion_1aa9e2f961c6dfdd5701fe614ab9b75604.md)

    Constructs one quaternion from values. 

* [Quaternion(const Float4 &v)](struct_luna_1_1_quaternion_1ad80f600bfac852235d03cee40af833a3.md)

    Constructs one quaternion from one vector. 

* [bool operator==(const Quaternion &q) const](struct_luna_1_1_quaternion_1ae4ff71d09a9f5a067e16cc751583b661.md)

    Compares two quaternions for equality. 

* [bool operator!=(const Quaternion &q) const](struct_luna_1_1_quaternion_1ab6a20c2bb7cb6a63d8d2657d41233376.md)

    Compares two quaternions for non-equality. 

* [Quaternion & operator=(const Float4 &v)](struct_luna_1_1_quaternion_1aed4a8ab53399a97c1788a2a85a494d18.md)

    Assigns one quaternion by coping components from one vector. 

* [Quaternion & operator+=(const Quaternion &q)](struct_luna_1_1_quaternion_1aa6a642c4f1b73088a7fcb3253658c3be.md)

    Adds this quaternion with one quaternion, and stores the result to this quaternion. 

* [Quaternion & operator-=(const Quaternion &q)](struct_luna_1_1_quaternion_1a386b83476234f02c63e4f87b77e79137.md)

    Subtracts this quaternion with one quaternion, and stores the result to this quaternion. 

* [Quaternion & operator*=(const Quaternion &q)](struct_luna_1_1_quaternion_1a45b5e33ccc03f4a050cc76b060e9c7d7.md)

    Concatenates two quaternions, and stores the result to this quaternion. 

* [Quaternion & operator*=(f32 s)](struct_luna_1_1_quaternion_1a605f32f1ecffc86baa144915310381d1.md)

    Multiplies this quaternion with one scalar, and stores the result to this quaternion. 

* [Quaternion & operator/=(const Quaternion &q)](struct_luna_1_1_quaternion_1a3afd1d575ecddc7d83d5d0bd43624954.md)

    Concatenates one inversed quaternion of `q` to this quaternions, and stores the result to this quaternion. 

* [Quaternion operator+() const](struct_luna_1_1_quaternion_1af8a79e99f42f923af485a34ad4121a39.md)

    Gets the quaternion as-is. 

* [Quaternion operator-() const](struct_luna_1_1_quaternion_1a4e44d502db7bfa4e5bbdda12f673d47a.md)

    Gets a negation of this quaternion. 

