# Luna::AHI::DeviceIODesc::adapter

```c++
IAdapter* adapter
```

The adapter bound to this stream. This adapter will be used to playback audio data from this stream, or capture audio data and write to this stream. If this is `nullptr`, the primary playback or capture device will be used. 

