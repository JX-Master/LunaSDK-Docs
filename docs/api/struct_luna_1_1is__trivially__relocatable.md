# Luna::is_trivially_relocatable
```c++
struct Luna::is_trivially_relocatable : public non-virtual std::integral_constant< bool, true >
```

## Overview
Checks if the specified type can be trivially relocatable. One object is trivially relocatable if the data of one well-constructed instance of object can be copied to a new uninitialized memory by bitwise copy (for example, `memcpy`, `memmove` or `realloc`) and the new copied object behaves the same as the original object, such copy is called a "relocating operation". After the operation, the original memory for the object is treated as uninitialized and does not have destructor called before it is freed.

If one object can be trivially relocated, then when the memory that holding the object needs to be reallocated (for example when the container needs to expand its capacity), it performs `memcpy`, `memmove` or any other bitwise copy algorithms directly on the data without any move constructors and destructors being called. If one object cannot be trivially relocated, then the relocating operation will call the move constructor for the object on the new memory (passing the old object as rvalue reference), then call the destructor for the old object to properly destruct itself before freeing the memory for the old object.

All objects are trivially relocatable unless the user explicitly creates a template specialization that evaluates this to `false_type` for the object that cannot be trivially relocated. In fact, the case that one type cannot be trivially relocatable is very rare, this only happens if the type holds a pointer to `this` and needs to update the pointer if the object is relocated. 

