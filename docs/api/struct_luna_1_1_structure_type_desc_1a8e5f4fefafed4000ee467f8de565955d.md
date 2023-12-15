# Luna::StructureTypeDesc::trivially_relocatable

```c++
bool trivially_relocatable
```

Whether this structure is trivially relocatable. One structure is trivially relocatable if its content can be moved to another memory address using memcpy, and using the instance on new memory location behaves the same as the instance on old memory location. 

