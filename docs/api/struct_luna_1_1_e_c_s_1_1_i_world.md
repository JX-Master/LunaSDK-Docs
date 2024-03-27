# Luna::ECS::IWorld
Represents one ECS context that holds entities and their components. Every world is independent to each other. 

```c++
interface Luna::ECS::IWorld : public virtual Interface
```



## Remark
The world object implements `IChangeList` as well. In such case, all calls to `IChangeList` behave like being committed immediately before return. The world itself is not thread safe, the user must ensure that modifications to the world are synchronized. 

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual Cluster * get_cluster(Span< const typeinfo_t > components, Span< const entity_id_t > tags, bool create_if_not_exist=false)=0](struct_luna_1_1_e_c_s_1_1_i_world_1a679ff80d2aa071c37f1911f2bcd0e724.md)

    Gets the cluster by components and tags. 

