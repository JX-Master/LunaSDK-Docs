# Luna::Blob
Represents one binary large object (BLOB). 

```c++
class Luna::Blob
```

## Overview
[Blob](class_luna_1_1_blob.md) can be used as a RAII wrapper for arbitrary memory allocation. One blob object allocates and manages one memory block that stores the blob data, which we call the "managed memory" of the blob object. The managed memory is always allocated from memalloc or memrealloc. The user can also allocate the memory manually then attach it to one blob object by calling Blob::attach, or call Blob::detach to take ownership of the managed memory from one blob object. 

