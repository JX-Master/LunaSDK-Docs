# Luna::AHI::capture_callback_t

```c++
using capture_callback_t =  void(const void* src_buffer, const WaveFormat& format, u32 num_frames)
```

Called when audio data is captured by the audio driver. The user should process such audio data (like coping them to application memory) if needed. 

This callback function is invoked in a dedicated audio thread, so the user must use synchronization mechanisms if needed. If this function takes too much time to return, some captured audio frames may be lost if the internal driver buffer is full. 

## Parameters
* *in* **src_buffer**

    The buffer to read audio frames from. The data read operation must not exceed `num_frames * get_frame_size(format.bit_depth, format.num_channels)` bytes. 

* *in* **format**

    The wave format of the audio data in `src_buffer`. 

* *in* **num_frames**

    The number of frames in `src_buffer`. 

