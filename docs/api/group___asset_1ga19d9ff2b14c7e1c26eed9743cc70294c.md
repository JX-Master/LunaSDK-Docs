# Luna::Asset::move_asset

```c++
RV move_asset(asset_t asset, const Path &new_path)
```

Moves all asset associated files to a new destination. 

This function performs the following tasks:1. Moves all files fetched from [get_asset_files](group___asset_1ga6f0d82ba87fd79c3932629c2d3c0cdf5.md) from old path to new path.

1. Changes path in asset metadata.

1. Saves modified asset metadata to asset metadata file. 

## Parameters
* *in* **asset**

    The asset handle of the asset to operate. 

* *in* **new_path**

    The new path of the asset. 

