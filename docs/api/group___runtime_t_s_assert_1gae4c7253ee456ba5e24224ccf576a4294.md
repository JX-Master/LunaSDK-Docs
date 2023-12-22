# lutsassert_lock

```c++
#define lutsassert_lock()
```

Defines a thread safe assertion lock that marks one structure or class type that should never be accessed by multiple threads without synchronization. 



## Remark
Add this macro to the body of one structure or class definition, and add [lutsassert](group___runtime_t_s_assert_1ga4922ccc9a32024a703fe3fddb61f9951.md) to member functions that should be protected. For example: 
```
// The non-thread-safe type.
class MyType
{
    lutsassert_lock();
    i32 value; // The data that should be accessed by only one thread.
    
    // Will crash the program if another thread is also calling functions of the same object
    // with lutsassert() set
    void set_value(i32 v)
    {
        lutsassert();
        value = v;
    }
    // 
    i32 get_value()
    {
        lutsassert();
        return value;
    }
};
```


