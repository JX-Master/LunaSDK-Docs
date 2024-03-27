# Luna::Asset::AssetTypeDesc::on_save_asset

```c++
RV(* on_save_asset) (object_t userdata, asset_t asset, const Path &path, object_t data)
```

Called when the asset data is being saved. 



## Parameters
* *in* **userdata**

    The userdata. 

* *in* **asset**

    The asset handle of the asset being saved. 

* *in* **path**

    The VFS path to save asset data to. 

* *in* **data**

    The asset data object to save. 

