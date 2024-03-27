# Luna::Asset::AssetState

```c++
enum AssetState
{
    unregistered= 0
    unloaded= 1
    loading= 2
    loaded= 3
}
```

Identifies the asset state. 

## Options
* [unregistered](group___asset_1ggab13244cbadc637f8b1d99534d1c4cc3ba7024db6aaf8e0fac22cd773f9b87f6bd.md)

    The asset handle is not registered. This asset should be registered first by calling [register_asset](group___asset_1ga2761d87367e59f0ff5d6e2726f21d800.md) or [new_asset](group___asset_1gaadb45644d9fc944348496f81119ea679.md). 

* [unloaded](group___asset_1ggab13244cbadc637f8b1d99534d1c4cc3ba5b2b01043b2bd78a7c1a811011197929.md)

    The asset data is not loaded. 

* [loading](group___asset_1ggab13244cbadc637f8b1d99534d1c4cc3baa14fa2166ed698f3d04061f57e5ab9b9.md)

    The asset data is loading. 

* [loaded](group___asset_1ggab13244cbadc637f8b1d99534d1c4cc3ba2430fe39e225818bd957ed4cb53eb770.md)

    The asset data is loaded. 

