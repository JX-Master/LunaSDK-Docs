# Luna::relocate_type

```c++
void relocate_type(typeinfo_t type, void *dst, void *src)
```

Relocates one instance of the specified type. 

The relocation is performed as follows:1. If `type` is a trivially relocatable type, use memcpy to move instance data.

1. If `type` is a non-trivially-relocatable type, use [move_construct_type](group___runtime_type_1gaedb52c18aad27367293256207fa535f0.md) to move construct one new instance on new location, then use [destruct_type](group___runtime_type_1ga89512f37edb473f255611970ac49d7d4.md) to destruct the old instance. 

## Parameters
### type
The type object. 

### dst
The pointer to the instance to be relocated. 

### src
The pointer to the new location of the instance. 

