# Luna::AHI::IDevice::add_capture_data_callback

```c++
virtual usize add_capture_data_callback(const Function< capture_callback_t > &callback)=0
```

Adds a callback that will be called when audio data is captured by the audio driver. 



## Remark
See [capture_callback_t](group___a_h_i_1gaadb71c72a4b7ed96ddc1ce91700a7aaf.md) for details. 

## Parameters
* *in* **callback**

    The callback to add. 

## Return value
Returns one handle that can be used to remove the added callback. 

