# Luna::Tuple
Represents a sequence of fixed-size elements. Every element can have one different type. 

```c++
template <typename _Ty, typename... _Tys>
class Luna::Tuple
```

Elements of one tuple type can be fetched by [get](group___runtime_1ga9aae6d134b69bdfb7f054dcd50ddf57c.md). 

## Member functions
* [Tuple()](class_luna_1_1_tuple_1a4766c7b239a3a6c3980f7e84d5439377.md)

    Constructs one tuple with every element being default-initialized. 

* [Tuple(const _Ty &arg1, const _Tys &... args)](class_luna_1_1_tuple_1a4843fd3efe97913cefad09232ac02c9f.md)

    Constructs one tuple with every element being copy-initialized. 

* [Tuple(_UTy1 &&arg1, _UTys &&... args)](class_luna_1_1_tuple_1a3dd06571fd4b87dc3b115ff9c0a8878e.md)

    Constructs one tuple with every element being converted from the specified value. 

* [Tuple(const Tuple< _UTy1, _UTys... > &rhs)](class_luna_1_1_tuple_1a987e05e1e8b35a96f5ee9188ddc958e4.md)

    Constructs one tuple by coping elements from another tuple. 

* [Tuple(Tuple< _UTy1, _UTys... > &&rhs)](class_luna_1_1_tuple_1a225c7a2bb3c842843a5a63def85f66a8.md)

    Constructs one tuple by moving elements from another tuple. 

* [Tuple(const Tuple &rhs)=default](class_luna_1_1_tuple_1acf1b28090d243a11c0f3d3974e391937.md)

    Constructs one tuple by coping elements from another tuple of the same type. 

* [Tuple(Tuple &&rhs)=default](class_luna_1_1_tuple_1a4c95c279acb3fb48c41f13007a4f078a.md)

    Constructs one tuple by moving elements from another tuple of the same type. 

* [Tuple & operator=(const Tuple &rhs)](class_luna_1_1_tuple_1aa5997789e9c667d63fede9fafc315187.md)

    Assigns elements of one tuple by coping elements from another tuple of the same type. 

* [Tuple & operator=(Tuple &&rhs)](class_luna_1_1_tuple_1abc1446595e9e8b0c2013398624e4f97c.md)

    Assigns elements of one tuple by moving elements from another tuple of the same type. 

* [Tuple & operator=(const Tuple< _UTy1, _UTys... > &rhs)](class_luna_1_1_tuple_1ac7222f5ff6ca3b77068d9f7d83d23c4e.md)

    Assigns elements of one tuple by coping elements from another tuple. 

* [Tuple & operator=(Tuple< _UTy1, _UTys... > &&rhs)](class_luna_1_1_tuple_1a2db0503505d9f1bffb218f56109e464b.md)

    Assigns elements of one tuple by moving elements from another tuple. 

* [bool operator==(const Tuple &rhs) const](class_luna_1_1_tuple_1a196b9f7e09ca4b5d0900b1139496a8a0.md)

    Compares two tuples for equality. 

* [bool operator!=(const Tuple &rhs) const](class_luna_1_1_tuple_1a37515513ea1645c01364172900baba25.md)

    Compares two tuples for non-equality. 

