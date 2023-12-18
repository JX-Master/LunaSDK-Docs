# Luna::RingDeque::shrink_to_fit

```c++
void shrink_to_fit()
```

Reduces the capacity of the queue so that [capacity](class_luna_1_1_ring_deque_1ad96bf59cb22e917cbd210ba068e8acb3.md) == [size](class_luna_1_1_ring_deque_1a79348f1b7c06b34052b42656a0279429.md). 

If [size](class_luna_1_1_ring_deque_1a79348f1b7c06b34052b42656a0279429.md) is `0`, this function releases the internal storage buffer. This can be used to clean up all dynamic memory allocated by this container. 

