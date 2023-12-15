# Luna::Path::append

```c++
void append(const Path &appended_path, usize pos)
```

Appends another path to the end of this path. 

## Overview
The flags and the root name of the appended path are ignored. 

## Parameters
### appended_path
The path to append. 

### pos
The index of the first node to append. Nodes in range [`appended_path.begin() + pos`, `appended_path.end()`) will be appended. 
