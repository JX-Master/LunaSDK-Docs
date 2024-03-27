# Luna::AHI::IDevice
Represents one audio device that can playback sounds. 

```c++
interface Luna::AHI::IDevice : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual u32 get_sample_rate()=0](struct_luna_1_1_a_h_i_1_1_i_device_1a235d01b9718656a932cbab4f3bad3f82.md)

    Gets the sample rate of the playback and capture stream. 

* [virtual DeviceFlag get_flags()=0](struct_luna_1_1_a_h_i_1_1_i_device_1acb80e6e1ec23428a0617eadcde6511ae.md)

    Gets device flags. 

* [virtual u32 get_playback_num_channels()=0](struct_luna_1_1_a_h_i_1_1_i_device_1a2688f33607a1134cd2f4fee750255f30.md)

    Gets the number of channels for the playback stream, which is also the number of audio samples in one audio frame. 

* [virtual BitDepth get_playback_bit_depth()=0](struct_luna_1_1_a_h_i_1_1_i_device_1aec8565f1274ed93165205959078f1876.md)

    Gets the bit depth of one sample in playback stream. 

* [virtual u32 get_capture_num_channels()=0](struct_luna_1_1_a_h_i_1_1_i_device_1a00be357023e8b796ad67961a542e4b2b.md)

    Gets the number of channels for the capture stream, which is also the number of audio samples in one audio frame. 

* [virtual BitDepth get_capture_bit_depth()=0](struct_luna_1_1_a_h_i_1_1_i_device_1af813c051cb6e75e3dc29d8305384b63b.md)

    Gets the bit depth of one sample in capture stream. 

* [virtual usize add_playback_data_callback(const Function< playback_callback_t > &callback)=0](struct_luna_1_1_a_h_i_1_1_i_device_1a16adab6e419f81fbb0b222d30d378cd1.md)

    Adds a callback that will be called when audio data is required by the audio driver for playback. 

* [virtual usize add_playback_data_callback(Function< playback_callback_t > &&callback)=0](struct_luna_1_1_a_h_i_1_1_i_device_1a2d0b689e2e449fcf11704844bdc91624.md)

    Adds a callback that will be called when audio data is required by the audio driver for playback. 

* [virtual void remove_playback_data_callback(usize handle)=0](struct_luna_1_1_a_h_i_1_1_i_device_1a27723d72bf5f1f4e8cf39c42bd48112e.md)

    Removes one callback added by [add_playback_data_callback](struct_luna_1_1_a_h_i_1_1_i_device_1a16adab6e419f81fbb0b222d30d378cd1.md). 

* [virtual usize add_capture_data_callback(const Function< capture_callback_t > &callback)=0](struct_luna_1_1_a_h_i_1_1_i_device_1a684e9bc69ddf964a33627de464983114.md)

    Adds a callback that will be called when audio data is captured by the audio driver. 

* [virtual usize add_capture_data_callback(Function< capture_callback_t > &&callback)=0](struct_luna_1_1_a_h_i_1_1_i_device_1af6eb564bcffb378fafb9897477adf97f.md)

    Adds a callback that will be called when audio data is captured by the audio driver. 

* [virtual void remove_capture_data_callback(usize handle)=0](struct_luna_1_1_a_h_i_1_1_i_device_1a1ac794b1a37de4402514618f34b848fe.md)

    Removes one callback added by [add_capture_data_callback](struct_luna_1_1_a_h_i_1_1_i_device_1a684e9bc69ddf964a33627de464983114.md). 

