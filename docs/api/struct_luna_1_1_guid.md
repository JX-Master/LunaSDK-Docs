# Luna::Guid
Represents a Globally Unique Identifier. 

```c++
struct Luna::Guid
```

## Overview
`[Guid](struct_luna_1_1_guid.md)` is a shortcut for Globally Unique Identifier. It is a 128-bit unsigned integer that is usually randomly generated and is used to identify one instance across multiple devices or domains.

`[Guid](struct_luna_1_1_guid.md)` can be constructed from a literal string that is formatted in its canonical textual representation, which appears like "xxxxxxxx-xxxx-Mxxx-Nxxx-xxxxxxxxxxxx". One open branket and one close branket may be added to the string, so both "123e4567-e89b-12d3-a456-426614174000" and "{123e4567-e89b-12d3-a456-426614174000}" are valid canonical textural representations of one `[Guid](struct_luna_1_1_guid.md)`.

See [https://en.wikipedia.org/wiki/Universally_unique_identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier) for details about GUID and its canonical textual representation. 

## Properties
* [u64 high](struct_luna_1_1_guid_1a815ac712840838394af17a580a826ce9.md)

    The high 64-bits of the GUID. 

* [u64 low](struct_luna_1_1_guid_1a5df88de4c741fbc3cdd8b4ea52218d4f.md)

    The low 64-bits of the GUID. 

