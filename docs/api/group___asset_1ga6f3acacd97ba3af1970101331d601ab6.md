# Luna::Asset::load_assets_meta

```c++
RV load_assets_meta(const Path &path, bool allow_overwrite=true)
```

Loads or reloads assets' metadata by reading asset metadata files. 



## Parameters
* *in* **path**

    The path of the asset or direcotry. If `path` specifies one asset, the system loads the asset metadata by opening its meta file and reading from it. If `path` specifies one directory, the system loads assets metadata for all assets in the directory recursively, every asset metadata is loaded as if `load_assets_meta` is called for that particular asset. 

* *in* **allow_overwrite**

    Specify the behavior when the specified asset already exists in the system. If `allow_overwrite` is `true`, the system will overwrite the asset metadata in the system using new asset metadata loaded from asset meta file; if `allow_overwrite` is `false`, the system discards the new asset metadata and does not change the asset metadata in the system if the specified asset already exists in the system. If `path` specifies one directory, this parameter is applied to all assets in that directory. 

