# Luna::WeakObjRef::get

```c++
object_t get() const
```

Gets the boxed object. 

This call does not modify the reference counter of the object. 

## Return value
Returns one pointer to the boxed object. Returns `nullptr` if the reference is null or the boxed object is expired. 

## Remark
It is not safe to use the returned boxed object directly, since one weak reference does not prevent one object from destructing itself if all strong references are released. This function only guarantees that the returned boxed object is valid when this function returns, but not after. To use the boxed object, the user should use [pin](class_luna_1_1_weak_obj_ref_1af6347ac675db0acd160d0b36e8418dfd.md) to create one strong reference from this reference, then use that reference instead. 

