# Luna::Asset::AssetTypeDesc::on_load_asset_default_data

```c++
R< ObjRef >(* on_load_asset_default_data) (object_t userdata, asset_t asset)
```

Called when one asset data object with default asset data is being requested. The user should create a new asset data object and load default asset data to the object. 

This function can be `nullptr`. If this function is `nullptr`, this asset type does not support loading default asset data, and such requests failed with BasicError::not_supported. 

## Parameters
* *in* **userdata**

    The userdata. 

* *in* **asset**

    The asset handle of the asset being loaded. 

## Return value
Returns the created asset data object with default asset data. 

