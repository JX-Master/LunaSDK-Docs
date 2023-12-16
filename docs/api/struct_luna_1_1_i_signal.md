# Luna::ISignal
Represents a system-level signal object. @threadsafe. 

```c++
interface Luna::ISignal : public virtual IWaitable
```

## Base type
* IWaitable
## Member functions
* [virtual void trigger()=0](struct_luna_1_1_i_signal_1a195530e6278298441214fa3b1ed938f3.md)

    Set this signal to trigged state. 

* [virtual void reset()=0](struct_luna_1_1_i_signal_1a20dcbdfbd0ec77afc802522bb7e379c1.md)

    Resets this signal to untriggered state for manual reset signals. 

