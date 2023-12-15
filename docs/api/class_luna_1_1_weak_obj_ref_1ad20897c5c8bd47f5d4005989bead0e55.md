# Luna::WeakObjRef::reset

```c++
void reset()
```

Resets the reference to null. 

This function decreases the weak reference counter of the boxed object before resetting the reference. If this reference is null when this function is called, this function does nothing. 

