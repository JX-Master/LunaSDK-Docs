# Luna::calculate_struct_memory_layout

```c++
void calculate_struct_memory_layout(Span< MemoryLayoutMember > members, usize &out_size, usize &out_alignment)
```

Calculates the size, alignment and memory layout for one structure type. 

## Overview
The calculated size, alignment and memory layout is compatible with C standard structure layout. 

## Parameters
### members
One span that provides members of the structure. 

### out_size
The calculated size of the structure. 

### out_alignment
The calculated alignment of the structure. 

