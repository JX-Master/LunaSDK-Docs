# Luna::AHI::get_adapters

```c++
RV get_adapters(Vector< Ref< IAdapter > > *playback_adapters, Vector< Ref< IAdapter > > *capture_adapters)
```

Gets a list of adapters (driver-provided audio devices) present on the platform. 



## Parameters
* *out* **playback_adapters**

    If not `nullptr`, returns all playback adapaters on the platform. 

* *out* **capture_adapters**

    If not `nullptr`, returns all capture adapaters on the platform. 

