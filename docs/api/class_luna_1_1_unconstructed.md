# Luna::Unconstructed
Represents one object that supports manual construction and destruction. 

```c++
template <typename _Ty>
class Luna::Unconstructed
```

`Unconstructed` provides a way to allocate the memory for a C++ object without their constructor/destructor being called by system. You have the ability to call their constructor/destructor manually. Such feature is useful when you need to declare some static constructed objects and want to control their construction/ destruction orders. Note that the `Unconstructed` class does not actually know if the object is constructed, you need to manage it manually and always call the destructor of the object when you want to destroy it. 

## Member functions
* [_Ty & get()](class_luna_1_1_unconstructed_1a38a9abd57df742d690f2ca0c668abab8.md)

    Get a reference to the object. 

* [const _Ty & get() const](class_luna_1_1_unconstructed_1a99f878496613323217993a6b57e6e7f6.md)

    Get a const reference to the object. 

* [void construct(Args &&... args)](class_luna_1_1_unconstructed_1a9cd3f54567668a517b7ca3df525e90c2.md)

    Constructs the object. 

* [void destruct()](class_luna_1_1_unconstructed_1af3b43681b3f195f17dac4f4ef64891f5.md)

    Destructs the object. 

