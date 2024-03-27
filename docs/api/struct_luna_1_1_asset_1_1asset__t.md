# Luna::Asset::asset_t
Represents one handle that identifies one asset entry in process scope. 

```c++
struct Luna::Asset::asset_t
```

An asset is one block of application data that is stored on one asset file. Every asset is identified by one asset GUID. The asset GUID is generated and assigned to one asset when the asset is created, and cannot be changed after the asset is created. The asset handle is the runtime representation of asset GUID. Every GUID has one unique asset handle, which can be fetched by [get_asset](group___asset_1gac941c1a7d0e790e712d2cb1cd2ffa2e6.md), the asset handle will be valid until the asset registry is closed, so we can always query asset information using one asset handle.

The main reason we use asset handle instead of using GUID directly to refer one asset is performance: the asset handle is actually one pointer to the internal asset entry information block, so we can fetch the asset information directly by dereferring the asset handle internally. If we use asset GUID instead, every asset information query call will have look up a global GUID-to-entry map to route the actual asset information block, which is slow and even slower in multi-threaded environment, since every look up to global GUID map must be synchronized.

The asset handle is unique in process scope, that is to say, if two processes (or restart the current process) refer to the same asset, their asset handle values are not the same. However, the asset GUID is unique globally, so that fetching assets using the same GUID will always get the same asset, even through their asset handle values may not be the same. Due to this reason, when serializing one reference to one asset, we should save the asset GUID rather than the handle value, so that we can get the same asset and restore reference after the application is restarted. 

