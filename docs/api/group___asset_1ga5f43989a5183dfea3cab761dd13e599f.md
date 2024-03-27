# Luna::Asset::save_asset

```c++
RV save_asset(asset_t asset)
```

Saves the asset data to files. 

This function saves the asset data synchronously. To save asset data asynchronously, call this function in the thread you want to use for asset saving, like a background thread or a worker thread in job system. 

## Parameters
* *in* **asset**

    The asset handle of the asset to operate. 

