# Asset
Runtime asset management system. 

## Topics
* [Asset Errors](asset_error.md)
## Types
* [Luna::Asset::asset_t](struct_luna_1_1_asset_1_1asset__t.md)

    Represents one handle that identifies one asset entry in process scope. 


* [Luna::Asset::AssetTypeDesc](struct_luna_1_1_asset_1_1_asset_type_desc.md)

    Describes one asset type. 


## Enumerations
* [Luna::Asset::AssetState](group___asset_1gab13244cbadc637f8b1d99534d1c4cc3b.md)

    Identifies the asset state. 

## Functions
* [void register_asset_type(const AssetTypeDesc &desc)](group___asset_1ga8c2349eaa35422a37f1a19dae31a54be.md)

    Registers one asset type so the asset system can handle the asset of that type. 

* [asset_t get_asset(const Guid &guid=Guid(0, 0))](group___asset_1gac941c1a7d0e790e712d2cb1cd2ffa2e6.md)

    Gets the asset handle from one asset GUID. If the asset entry with the specified GUID does not exist, this function creates one new asset entry with the specified GUID and returns the handle to the new created asset entry. 

* [RV register_asset(asset_t asset, const Name &type)](group___asset_1ga2761d87367e59f0ff5d6e2726f21d800.md)

    Registers the specified asset. 

* [R< asset_t > new_asset(const Path &path, const Name &type, bool save_meta_to_file=true)](group___asset_1gaadb45644d9fc944348496f81119ea679.md)

    Creates a new asset by specifying the path and type of the asset. 

* [RV load_assets_meta(const Path &path, bool allow_overwrite=true)](group___asset_1ga6f3acacd97ba3af1970101331d601ab6.md)

    Loads or reloads assets' metadata by reading asset metadata files. 

* [RV load_asset_meta(asset_t asset)](group___asset_1ga46de33b70b37511bae7051ae93b67387.md)

    Loads asset metadata from asset's metadata file. 

* [RV save_asset_meta(asset_t asset)](group___asset_1ga1477c0674fba3bcd108ab7c7909e410c.md)

    Saves asset's metadata to asset's metadata file. 

* [R< asset_t > get_asset_by_path(const Path &path)](group___asset_1ga7241b8a9f8260a48b2a0acc08149dd56.md)

    Gets one asset by path. 

* [Guid get_asset_guid(asset_t asset)](group___asset_1gae8579cf0a5b471fa78696529801d92e9.md)

    Gets the asset GUID. 

* [Path get_asset_path(asset_t asset)](group___asset_1ga33d922e7b67edc3a7d391ad28695ee37.md)

    Gets the asset VFS path. 

* [RV set_asset_path(asset_t asset, const Path &path)](group___asset_1ga869a52b900e0c81f7a094336340464f6.md)

    Sets the asset VFS path. 

* [Name get_asset_name(asset_t asset)](group___asset_1ga98716b6dd29950ba6304d114c83d3435.md)

    Gets the asset name, which is the filename component of the asset VFS path, excluding the extension. 

* [Name get_asset_type(asset_t asset)](group___asset_1gab3beb91f7c68d8d60daf7997862815e9.md)

    Gets the asset type. 

* [void set_asset_type(asset_t asset, const Name &type)](group___asset_1ga5f2e84af094678a3d5388eb54284378b.md)

    Sets the asset type. 

* [RV get_asset_files(asset_t asset, Vector< Name > &filenames)](group___asset_1ga6f0d82ba87fd79c3932629c2d3c0cdf5.md)

    Get filenames of all files associated to the specified asset. 

* [RV delete_asset(asset_t asset)](group___asset_1gae2363518042514cec6f2afc53d6bfd00.md)

    Deletes one asset and all of its associated files. 

* [RV move_asset(asset_t asset, const Path &new_path)](group___asset_1ga19d9ff2b14c7e1c26eed9743cc70294c.md)

    Moves all asset associated files to a new destination. 

* [ObjRef get_asset_data(asset_t asset)](group___asset_1gac59ffaac732391031af05d984dcb08aa.md)

    Gets the asset data object. 

* [Ref< _Ty > get_asset_data(asset_t asset)](group___asset_1ga9603d71e11ed28c38c0c62e64546e3a2.md)

    Gets the asset data object. 

* [RV set_asset_data(asset_t asset, object_t data)](group___asset_1gaf3ec1421837a85365d67c57334640fbf.md)

    Sets the asset data object. 

* [RV load_asset(asset_t asset, bool force_reload=false)](group___asset_1ga5288cafda7e01d50857485b3798d707e.md)

    Creates one asset data object for the asset by loading data from asset file. 

* [RV load_asset_default_data(asset_t asset, bool force_reload=false)](group___asset_1gae20453da814d6e55763771d3c44372a3.md)

    Creates one asset data object for the asset by loading default asset data. 

* [AssetState get_asset_state(asset_t asset)](group___asset_1gaee4164c941084a29087e9edb2ffe8398.md)

    Gets the asset state. 

* [RV save_asset(asset_t asset)](group___asset_1ga5f43989a5183dfea3cab761dd13e599f.md)

    Saves the asset data to files. 

* [void close()](group___asset_1ga5ae591df94fc66ccb85cbb6565368bca.md)

    Closes the asset registry. 

