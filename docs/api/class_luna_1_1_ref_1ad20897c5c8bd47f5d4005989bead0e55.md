# Luna::Ref::reset

```c++
void reset()
```

Resets the reference to null. 

## Overview
This function decreases the strong reference counter of the boxed object before resetting the reference. If this reference is null when this function is called, this function does nothing. 

