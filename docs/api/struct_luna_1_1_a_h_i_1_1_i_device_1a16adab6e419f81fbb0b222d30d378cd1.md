# Luna::AHI::IDevice::add_playback_data_callback

```c++
virtual usize add_playback_data_callback(const Function< playback_callback_t > &callback)=0
```

Adds a callback that will be called when audio data is required by the audio driver for playback. 



## Remark
See [playback_callback_t](group___a_h_i_1ga3665f39ee93f794913a4ac328c3dd090.md) for details. 

## Parameters
* *in* **callback**

    The callback to add. 

## Return value
Returns one handle that can be used to remove the added callback. 

