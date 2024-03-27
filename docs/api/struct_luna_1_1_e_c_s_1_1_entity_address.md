# Luna::ECS::EntityAddress
Describes the entity address. The address of the entity will change when structural changes are performed to the world. 

```c++
struct Luna::ECS::EntityAddress
```

## Member objects
* [Cluster* cluster](struct_luna_1_1_e_c_s_1_1_entity_address_1a3f1a3b821b2f0c4f7614df1901dbaaf6.md)

    The cluster that the entity belongs to. One cluster records one array of entities with the same components and tags. 

* [usize index](struct_luna_1_1_e_c_s_1_1_entity_address_1a46266689dc5df0720190686fb20efb80.md)

    The index of the entity in the archetype array. 

