# Luna::Name
Represents one name string. 

```c++
class Luna::Name
```

The name string is one constant string that is mainly used to identify entities in LunaSDK. [Name](class_luna_1_1_name.md) strings are reference counted and managed by system, all [Name](class_luna_1_1_name.md) objects containing the same name string will refer the same name internal string data, enabling fast comparison: instead of comparing the whole string, we only need to compare one pointer to determine whether two name strings are the same. 

## Member functions
* [Name()](class_luna_1_1_name_1aee637aaac62ffd89b7b7c6b6529e913b.md)

    Constructs one empty name. 

* [Name(const c8 *name)](class_luna_1_1_name_1a1a1d629fd8da2800e7153328215c852f.md)

    Constructs one name with the provided name string. 

* [Name(const c8 *name, usize count)](class_luna_1_1_name_1a7c6e6c238815764353cb0cf8f20d9de0.md)

    Constructs one name with the provided name string and size. 

* [Name(const String &str)](class_luna_1_1_name_1a711553d241082264643b3a61e70b8cb6.md)

    Constructs one name from one string. 

* [Name(const String &str, usize pos, usize count)](class_luna_1_1_name_1a97b5bb171560e992a13a551821f9b73b.md)

    Constructs one name from one substring of the provided string. 

* [const c8 * c_str() const](class_luna_1_1_name_1a5ad81a0d755899f04deb6fd793bb27f6.md)

    Gets the internal string pointer of this name. 

* [usize size() const](class_luna_1_1_name_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the name string. 

* [name_id_t id() const](class_luna_1_1_name_1a610a3ab098fb008aad0478beea601a76.md)

    Gets the ID of the name string. 

* [bool empty() const](class_luna_1_1_name_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this name string is empty. 

* [operator bool() const](class_luna_1_1_name_1a67b76affb3b5d35fa419ac234144038b.md)

    Checks whether this name string is empty. 

* [void reset()](class_luna_1_1_name_1ad20897c5c8bd47f5d4005989bead0e55.md)

    Clears the name string and resets it to one empty name. 

* [bool operator==(const Name &rhs) const](class_luna_1_1_name_1a970adff199cd33d49ec88821e8d5ef98.md)

    Compares two names for equality. 

* [bool operator!=(const Name &rhs) const](class_luna_1_1_name_1af3a1e19372a372acc6afb54dea79fadc.md)

    Compares two names for non-equality. 

* [operator String() const](class_luna_1_1_name_1ad2500b704d297c0a2cde6256112d770e.md)

    Converts one name to one string. 

