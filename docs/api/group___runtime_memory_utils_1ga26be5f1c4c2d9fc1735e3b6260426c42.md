# Luna::calculate_union_memory_layout

```c++
void calculate_union_memory_layout(Span< MemoryLayoutMember > members, usize &out_size, usize &out_alignment)
```

Calculates the size, alignment and memory layout for one union type. 

## Overview
The calculated size, alignment and memory layout is compatible with C standard union layout. 

## Parameters
### members
One span that provides members of the union. 

### out_size
The calculated size of the union. 

### out_alignment
The calculated alignment of the union. 

