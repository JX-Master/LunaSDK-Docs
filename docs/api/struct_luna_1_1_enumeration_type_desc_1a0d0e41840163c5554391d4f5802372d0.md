# Luna::EnumerationTypeDesc::multienum

```c++
bool multienum
```

## Overview
Whether this enumeration is a multi-value enumeration. A multi-value enumeration uses one unique bit of the value for every possible option, while a single-value enumeration uses one unique value for every possible option. For example, for one enumeration with `u16` underlying type, 16 possible options may present if the enumeration is a multi-value enumeration, and 65536 possible options may present if the enumeration is a noral enumeration. 

