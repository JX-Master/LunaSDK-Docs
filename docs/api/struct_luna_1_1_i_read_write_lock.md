# Luna::IReadWriteLock
Represents one system-level read write lock. 

```c++
interface Luna::IReadWriteLock : public virtual Interface
```

One read write lock allows multiple threads to access the same resource in read mode, or at most one thread to access the resource in write mode. One read write lock is created in unlocked mode, and can be transferred to read mode by acquiring read ownership of the lock, or transferred to write mode by acquiring write ownership of the lock. When the read write lock is in read mode, successing acquires of read ownership succeeds, but acquires of write ownership will fail or be blocked until all read ownerships are released; When the read write lock is in write mode, all succeeding acquires of read and write ownerships will fail or be blocked until the write ownership is released. The write ownership is not recursive: succeeding acquire of write ownership from the thread that already acquired the write ownership causes deadlock and shall not be performed. This\ type\ is\ thread\ safe. 

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual void acquire_read()=0](struct_luna_1_1_i_read_write_lock_1a4c422b9f02a7acdbc1b18668d0d4fa9f.md)

    Acquires one read ownership of the lock. 

* [virtual void acquire_write()=0](struct_luna_1_1_i_read_write_lock_1abdaf802022253a2a516731180958b4c5.md)

    Acquires one write ownership of the lock. 

* [virtual bool try_acquire_read()=0](struct_luna_1_1_i_read_write_lock_1affc9612ed2c089bba5dadf527a42acb8.md)

    Tries to acquire one read ownership of the lock. 

* [virtual bool try_acquire_write()=0](struct_luna_1_1_i_read_write_lock_1aaafad82e226eb10829ab823b3fb49da6.md)

    Tries to acquire one write ownership of the lock. 

* [virtual void release_read()=0](struct_luna_1_1_i_read_write_lock_1a4ae8f05cc92bc1c6ec3069ef8a79b590.md)

    Releases the read ownership acquired by [acquire_read](struct_luna_1_1_i_read_write_lock_1a4c422b9f02a7acdbc1b18668d0d4fa9f.md) or [try_acquire_read](struct_luna_1_1_i_read_write_lock_1affc9612ed2c089bba5dadf527a42acb8.md). 

* [virtual void release_write()=0](struct_luna_1_1_i_read_write_lock_1ae2a34e31690b2e76292eb05389dfa36f.md)

    Releases the write ownership acquired by [acquire_write](struct_luna_1_1_i_read_write_lock_1abdaf802022253a2a516731180958b4c5.md) or [try_acquire_write](struct_luna_1_1_i_read_write_lock_1aaafad82e226eb10829ab823b3fb49da6.md). 

