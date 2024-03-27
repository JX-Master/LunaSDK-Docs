# Luna::RHI::BufferBarrier
Describes one buffer barrier. 

```c++
struct Luna::RHI::BufferBarrier
```

## Member objects
* [IBuffer* buffer](struct_luna_1_1_r_h_i_1_1_buffer_barrier_1a66b6e32a2ca728d104d46a04a74e4f09.md)

    The resource the barrier is applied to. 

* [BufferStateFlag before](struct_luna_1_1_r_h_i_1_1_buffer_barrier_1a85c81c2f49bd4a81ab5093dd30cee82f.md)

    The states of the resource before this barrier takes place. Specify [BufferStateFlag::automatic](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda2bd9c0ed00116be1258e0cc66617d7c8.md) to let the system decide the before state, see docs of [BufferStateFlag::automatic](group___r_h_i_1gga44197ca8c7fae3c510e42a6c9b5536bda2bd9c0ed00116be1258e0cc66617d7c8.md) for details. 

* [BufferStateFlag after](struct_luna_1_1_r_h_i_1_1_buffer_barrier_1a1410c0e1ced23d1ca1419ea85729bbb3.md)

    The states of the resource after this barrier takes place. 

* [ResourceBarrierFlag flags](struct_luna_1_1_r_h_i_1_1_buffer_barrier_1a0b56e6520415e72031407a344fce80a4.md)

    Additional flags for this barrier. 

