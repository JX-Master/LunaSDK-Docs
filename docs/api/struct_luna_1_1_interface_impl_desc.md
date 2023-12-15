# Luna::InterfaceImplDesc
Describes arguments to register an interface implementation. 

```c++
struct Luna::InterfaceImplDesc
```

## Properties
* [Guid type_guid](struct_luna_1_1_interface_impl_desc_1ae9a2220557b7ef8a4db71662ce9becea.md)

    The GUID of the type that implements the interface. 

* [Guid interface_guid](struct_luna_1_1_interface_impl_desc_1a6bfe519e6f8338499457ee013993f8ce.md)

    The GUID of the interface. 

* [void *(* cast_to_interface) (object_t obj)](struct_luna_1_1_interface_impl_desc_1aeb605cc0af8fe3560a6bd05a635cd142.md)

    The function pointer called to cast the object pointer to the specified interface pointer. 

