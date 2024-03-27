# Luna::Asset::AssetTypeDesc::on_set_asset_data

```c++
RV(* on_set_asset_data) (object_t userdata, asset_t asset, object_t data)
```

Called when a new asset data object is set to the specified asset. 

This function is called before the set operation happens, so the user can call [get_asset_data](group___asset_1gac59ffaac732391031af05d984dcb08aa.md) on `asset` to get the existing asset data object (if any).

If this function fails, the new asset data object will not be set, that the existing asset data object is not changed.

This function can be `nullptr`, in such case, the default callback function will be used, which simply does nothing and returns success directly. 

## Parameters
* *in* **userdata**

    The userdata. 

* *in* **asset**

    The asset handle of the asset to set new asset data object. 

* *in* **data**

    The new asset data object to set. This can be `nullptr` if the user calls [set_asset_data](group___asset_1gaf3ec1421837a85365d67c57334640fbf.md) with `data` equals to `nullptr`. In such case, this function behaves like unloading existing asset data object. 

