# Luna::AHI::IAdapter
Represents one audio adapter that can be used to create one device. 

```c++
interface Luna::AHI::IAdapter : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual const c8 * get_name()=0](struct_luna_1_1_a_h_i_1_1_i_adapter_1ae34a0f761c133b9052bd44d4bdf71271.md)

    Gets the name of this adapter. 

* [virtual bool is_primary()=0](struct_luna_1_1_a_h_i_1_1_i_adapter_1a47bb44eb809780b2b2918fdad4af6d8b.md)

    Checks if this adapter is the primary adapter of the platform. 

* [virtual RV get_native_wave_formats(WaveFormat *out_formats, usize *num_formats)=0](struct_luna_1_1_a_h_i_1_1_i_adapter_1a5db4174545d1e5f5962425c41506526b.md)

    Gets a list of native wave formats supported by this adapter. 

