# Interfaces
## Types
* [Luna::InterfaceImplDesc](struct_luna_1_1_interface_impl_desc.md)

    Describes arguments to register an interface implementation. 


* [Luna::Interface](struct_luna_1_1_interface.md)

    The base interface for all other interfaces in Luna SDK. 


## Functions
* [void impl_interface_for_type(const InterfaceImplDesc &desc)](group___runtime_interface_1ga945dc30f32030f88b5df4e99a04cdeb4.md)

    Registers one interface implementation. 

* [void impl_interface_for_type()](group___runtime_interface_1ga44b21a1d55c2f93cc3cb96657f88d690.md)

    Registers one or more interface implementations for one type. 

* [bool is_interface_implemented_by_type(typeinfo_t type, const Guid &iid)](group___runtime_interface_1ga351ebc4eab8cce713963e130a1fcec0f.md)

    Checks whether the specified type implements the specified interface. 

* [void * query_interface(object_t object, const Guid &iid)](group___runtime_interface_1ga86b6ea2b9c911ba917462d3797e174d4.md)

    Gets one interface pointer from one pointer to one boxed object that implements the interface. 

* [_Ity * query_interface(object_t object)](group___runtime_interface_1gaf6fa36ce4224a745157d50c5c618b32e.md)

    Gets one interface pointer from one pointer to one boxed object that implements the interface. 

