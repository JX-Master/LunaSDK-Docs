# Luna::Asset::AssetTypeDesc::on_load_asset

```c++
R< ObjRef >(* on_load_asset) (object_t userdata, asset_t asset, const Path &path)
```

Called when one asset data object with data loaded from the specified file is being requested. The user should create a new asset data object and load asset data from the specified file to the object. 

This function can be `nullptr`. If this function is `nullptr`, this asset type does not support loading asset data from file, and such requests failed with BasicError::not_supported. 

## Parameters
* *in* **userdata**

    The userdata. 

* *in* **asset**

    The asset handle of the asset being loaded. 

* *in* **path**

    The VFS path to load asset data from. 

## Return value
Returns the loaded asset data object. 

