# Luna::RHI::TextureBarrier
Describes one texture barrier. 

```c++
struct Luna::RHI::TextureBarrier
```

## Member objects
* [ITexture* texture](struct_luna_1_1_r_h_i_1_1_texture_barrier_1ab02abc67d0395436de0c53aca08fd08f.md)

    The resource the barrier is applied to. 

* [SubresourceIndex subresource](struct_luna_1_1_r_h_i_1_1_texture_barrier_1ac40b611350f8a22fb009fd9d050480a8.md)

    The subresource in the resource the barrier is applied to. Specify [TEXTURE_BARRIER_ALL_SUBRESOURCES](group___r_h_i_1gae1ebf3b256a5d406c1fd4ef77f508572.md) will apply the barrier to all subresources of the resource. 

* [TextureStateFlag before](struct_luna_1_1_r_h_i_1_1_texture_barrier_1a07ba9c68cf7dcab846e764d29b5210be.md)

    The states of the [subresource(s)](struct_luna_1_1_r_h_i_1_1_texture_barrier_1ac40b611350f8a22fb009fd9d050480a8.md) before this barrier takes place. Specify [TextureStateFlag::automatic](group___r_h_i_1ggabfe469f739b00632e7855e0b9e775fe6a2bd9c0ed00116be1258e0cc66617d7c8.md) to let the system decide the before state, see docs of [TextureStateFlag::automatic](group___r_h_i_1ggabfe469f739b00632e7855e0b9e775fe6a2bd9c0ed00116be1258e0cc66617d7c8.md) for details. 

* [TextureStateFlag after](struct_luna_1_1_r_h_i_1_1_texture_barrier_1a6dc5e04645d9b0d76d8a1c552b5feb50.md)

    The states of the [subresource(s)](struct_luna_1_1_r_h_i_1_1_texture_barrier_1ac40b611350f8a22fb009fd9d050480a8.md) after this barrier takes place. 

* [ResourceBarrierFlag flags](struct_luna_1_1_r_h_i_1_1_texture_barrier_1a0b56e6520415e72031407a344fce80a4.md)

    Additional flags for this barrier. 

