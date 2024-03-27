# Luna::ObjLoader::load

```c++
R< ObjMesh > load(Span< const byte_t > obj_file, Span< const byte_t > mtl_file={})
```

Loads mesh from OBJ file data. 



## Parameters
* *in* **obj_file**

    The object file (.obj) data. 

* *in* **mtl_file**

    The material file (.mtl) data. This is optional. 

## Return value
Returns the loaded mesh data. 

