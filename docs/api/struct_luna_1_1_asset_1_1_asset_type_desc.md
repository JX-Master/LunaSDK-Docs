# Luna::Asset::AssetTypeDesc
Describes one asset type. 

```c++
struct Luna::Asset::AssetTypeDesc
```

## Member objects
* [Name name](struct_luna_1_1_asset_1_1_asset_type_desc_1a7082db574ba2d2d69ccafb060398b7d8.md)

    The asset type name. 

* [ObjRef userdata](struct_luna_1_1_asset_1_1_asset_type_desc_1a2d82fc587187f7512fe0aa007b6dc304.md)

    The userdata object. The object will be kept by the asset system and provided to every callback function. 

* [R< ObjRef >(* on_load_asset) (object_t userdata, asset_t asset, const Path &path)](struct_luna_1_1_asset_1_1_asset_type_desc_1a0132cc1cd018fee4e1d748cdca2fbeff.md)

    Called when one asset data object with data loaded from the specified file is being requested. The user should create a new asset data object and load asset data from the specified file to the object. 

* [R< ObjRef >(* on_load_asset_default_data) (object_t userdata, asset_t asset)](struct_luna_1_1_asset_1_1_asset_type_desc_1a0ce7cdc768d64c311ea62002aa62b415.md)

    Called when one asset data object with default asset data is being requested. The user should create a new asset data object and load default asset data to the object. 

* [RV(* on_save_asset) (object_t userdata, asset_t asset, const Path &path, object_t data)](struct_luna_1_1_asset_1_1_asset_type_desc_1ad408c9ddaf37d2c40fc5851944780321.md)

    Called when the asset data is being saved. 

* [RV(* on_set_asset_data) (object_t userdata, asset_t asset, object_t data)](struct_luna_1_1_asset_1_1_asset_type_desc_1a93afd88f5caf3fa66d20e8005fa712cf.md)

    Called when a new asset data object is set to the specified asset. 

