# Luna::new_signal

```c++
Ref< ISignal > new_signal(bool manual_reset)
```

Create a new signal object. 



## Parameters
* *in* **manual_reset**

    If we need to manually reset the trigger state of the signal object. If set to `false`, the signal will be automatically reset to not triggered state when a single thread that waiting for this signal is passed. If set to `true`, user needs to manually reset the state by calling [ISignal::reset](struct_luna_1_1_i_signal_1a20dcbdfbd0ec77afc802522bb7e379c1.md). 

## Return value
Returns the new created signal object. 

