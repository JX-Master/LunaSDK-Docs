# Luna::Asset::delete_asset

```c++
RV delete_asset(asset_t asset)
```

Deletes one asset and all of its associated files. 

This function performs the following tasks:1. Delete all files fetched from [get_asset_files](group___asset_1ga6f0d82ba87fd79c3932629c2d3c0cdf5.md).

1. Set asset path, type and data object to empty. The asset handle will still be valid after this operation, but the asset state will be set to [AssetState::unregistered](group___asset_1ggab13244cbadc637f8b1d99534d1c4cc3ba7024db6aaf8e0fac22cd773f9b87f6bd.md), and all operations to the asset is invalid. 

## Parameters
* *in* **asset**

    The asset handle of the asset to operate. 

