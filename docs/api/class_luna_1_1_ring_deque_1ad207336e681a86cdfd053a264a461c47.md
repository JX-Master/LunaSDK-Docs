# Luna::RingDeque::RingDeque

```c++
RingDeque(RingDeque &&rhs, const allocator_type &alloc)
```

Constructs a queue with an custom allocator and with elements moved from another queue. 



## Parameters
* *in* **rhs**

    The queue to move elements from. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the queue. 

