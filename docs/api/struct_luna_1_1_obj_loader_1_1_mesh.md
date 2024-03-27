# Luna::ObjLoader::Mesh
Describes the mesh data of one shape. 

```c++
struct Luna::ObjLoader::Mesh
```

## Member objects
* [Vector<Index> indices](struct_luna_1_1_obj_loader_1_1_mesh_1ab770172d08d85fafd19833d31b0038e6.md)

    The indices of vertices of this mesh. 

* [Vector<u8> num_face_vertices](struct_luna_1_1_obj_loader_1_1_mesh_1aebb5269167a82b91db2abda6fcf653f7.md)

    The number of vertices per face. 3 = triangle, 4 = quad, ... Up to 255 vertices per face. 

* [Vector<i32> material_ids](struct_luna_1_1_obj_loader_1_1_mesh_1aa7b7c4605c7a9e2504fa140d9332af65.md)

    per-face material ID 

