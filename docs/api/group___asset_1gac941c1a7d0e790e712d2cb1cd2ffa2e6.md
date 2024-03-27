# Luna::Asset::get_asset

```c++
asset_t get_asset(const Guid &guid=Guid(0, 0))
```

Gets the asset handle from one asset GUID. If the asset entry with the specified GUID does not exist, this function creates one new asset entry with the specified GUID and returns the handle to the new created asset entry. 

Asset handles created by [get_asset](group___asset_1gac941c1a7d0e790e712d2cb1cd2ffa2e6.md) is in unregistered state ( [get_asset_state](group___asset_1gaee4164c941084a29087e9edb2ffe8398.md) returns [AssetState::unregistered](group___asset_1ggab13244cbadc637f8b1d99534d1c4cc3ba7024db6aaf8e0fac22cd773f9b87f6bd.md)). The user should call [register_asset](group___asset_1ga2761d87367e59f0ff5d6e2726f21d800.md) on the handle to register the asset before she can really use the asset. The user can also call [new_asset](group___asset_1gaadb45644d9fc944348496f81119ea679.md) to create and register asset in one call. 

## Parameters
* *in* **guid**

    The asset GUID to fetch. If this is (0, 0), the system generates a random asset GUID, so that one new asset entry is always created and returned. 

## Return value
Returns the asset handle with the specified GUID. 

