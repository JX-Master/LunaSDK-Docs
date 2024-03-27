# Luna::ECS::IWorld::get_cluster

```c++
virtual Cluster * get_cluster(Span< const typeinfo_t > components, Span< const entity_id_t > tags, bool create_if_not_exist=false)=0
```

Gets the cluster by components and tags. 

