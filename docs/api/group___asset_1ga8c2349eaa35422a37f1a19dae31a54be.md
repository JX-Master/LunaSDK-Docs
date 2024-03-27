# Luna::Asset::register_asset_type

```c++
void register_asset_type(const AssetTypeDesc &desc)
```

Registers one asset type so the asset system can handle the asset of that type. 

If one asset type with the same name already exists, the existing asset type will be replaced with the new asset type. 

## Parameters
* *in* **desc**

    The asset type descriptor. 

