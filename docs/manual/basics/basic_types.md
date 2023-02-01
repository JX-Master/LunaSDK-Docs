# Basic Types

## Primitive typesThe following table lists all primitive typed designed by Luna SDK.

| Type    | Description                     | C++ STD Equivalent |
| ------- | ------------------------------- | ------------------ |
| `u8`    | Unsigned 8-bit integer.         | `std::uint8_t`     |
| `i8`    | Signed 8-bit integer.           | `std::int8_t`      |
| `u16`   | Unsigned 16-bit integer.        | `std::uint16_t`    |
| `i16`   | Signed 16-bit integer.          | `std::int16_t`     |
| `u32`   | Unsigned 32-bit integer.        | `std::uint32_t`    |
| `i32`   | Signed 32-bit integer.          | `std::int32_t`     |
| `u64`   | Unsigned 64-bit integer.        | `std::uint64_t`    |
| `i64`   | Signed 64-bit integer.          | `std::int64_t`     |
| `usize` | Unsigned machine-sized integer. | `std::size_t`      |
| `isize` | Signed machine-sized integer.   | `std::ptrdiff_t`   |
| `f32`   | 32-bit floating-point number.   | `float`            |
| `f64`   | 64-bit floating-point number.   | `double`           |
| `c8`    | 8-bit character.                | `char`             |
| `c16`   | 16-bit character.               | `chat16_t`         |
| `c32`   | 32-bit character.               | `char32_t`         |

## Containers

```c++
#include <Runtime/Vector.hpp>
#include <Runtime/List.hpp>
#include <Runtime/HashMap.hpp>
#include <Runtime/HashSet.hpp>
#include <Runtime/UnorderedMap.hpp>
#include <Runtime/UnorderedSet.hpp>
#include <Runtime/UnorderedMultiMap.hpp>
#include <Runtime/UnorderedMultiSet.hpp>
#include <Runtime/SelfIndexedHashMap.hpp>
#include <Runtime/SelfIndexedUnorderedMap.hpp>
#include <Runtime/SelfIndexedUnorderedMultiMap.hpp>
#include <Runtime/RingDeque.hpp>
```

For compatibility and cross-platform consistency reasons, Luna SDK does not use C++ Standard Template Library (STD), but implements its own container types using APIs similar to those of STD. The following table lists all containers provided by Luna SDK.

| Container Type                          | Description                                                  | C++ STD Equivalent              |
| --------------------------------------- | ------------------------------------------------------------ | ------------------------------- |
| `Vector<T>`                             | Dynamic array type.                                          | `std::vector<T>`                |
| `List<T>`                               | Dynamic double-linked list type.                             | `std::list<T>`                  |
| `HashMap<K, V>`                         | Closed hash map type using Robinhood Hashing.                | N/A                             |
| `HashSet<V>`                            | Closed hash set type using Robinhood Hashing.                | N/A                             |
| `UnorderedMap<K, V>`                    | Open hash map type.                                          | `std::unordered_map<K, V>`      |
| `UnorderedSet<V>`                       | Open hash set type.                                          | `std::unordered_set<V>`         |
| `UnorderedMultiMap<K, V>`               | Open hash map type that allows elements with the same key.   | `std::unordered_multimap<K, V>` |
| `UnorderedMultiSet<V>`                  | Open hash map type that allows multiple insertions of the same elements. | `std::unordered_multiset<K, V>` |
| `SelfIndexedHashMap<K, V, E>`           | Closed hash map whose key type can be extracted from the value type. | N/A                             |
| `SelfIndexedUnorderedMap<K, V, E>`      | Open hash map whose key type can be extracted from the value type. | N/A                             |
| `SelfIndexedUnorderedMultiMap<K, V, E>` | Open hash map whose key type can be extracted from the value type, and allows multiple insertions of the same elements. | N/A                             |
| `RingDeque<T>`                          | Double-ended queue using ring buffering.                     | `std::deque<T>`                 |

### Self indexed map containers

Self indexed map containers are used for elements whose key is a part of the value object. For example, given the following structure:

```c++
struct Player
{
	Name name;
	i32 hp;
    i32 mp;
};
```

Now we want to use one map to store all player records using their name as the key. If we use normal `HashMap` or `UnorderedMap` container, every entry in the container will be saved as `Pair<const Name, Player>`, thus stores the player name twice. In such case, we can use `SelfIndexedHashMap` and `SelfIndexedUnorderedMap` instead. The self indexed hash map container does not store the key object directly, instead, it requires the user to provide a special functional object `E`, which will be called when the key is needed. The functional object `E` takes a reference to the value object of the map element, and should returns a value or reference to the key object of the element. In our example, we can implement `E` as below:

```c++
struct PlayerExtractKey
{
	const Name& operator()(const Player& val) const
	{
		return val.name;
	}
};
```

Then we can define the self indexed map like so:

```c++
#include <Runtime/SelfIndexedHashMap.hpp>

namespace Luna
{
	SelfIndexedHashMap<Name, Player, PlayerExtractKey> players;
}
```

When using self indexed map containers, the user must ensure that the key object is immutable for all elements in the container, or the behavior is undefined.

## GUID

```c++
#include <Runtime/Base.hpp>
```

Globally Unique Identifier (GUID) is a algorithm-generated 128-bit integer identifier. In Luna SDK, GUIDs are represented by `Guid` type:

```c++
struct Guid
{
	u64 high;
	u64 low;
};
```

Luna SDK supports generating GUID instances from the registry form (`xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` or `{xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx}`) at compile time:

```c++
constexpr Guid test_id("{5cf28858-60b0-49f2-9674-5888fa7ad027}");
static_assert(test_id.low == 10841387548328775719Ui64, "Incorrect GUID values.");
static_assert(test_id.high == 6697565509014014450Ui64, "Incorrect GUID values.");
```

GUIDs are used widely in Luna SDK for identifying assets, types, interfaces, objects and many other entities.

## Version type

```c++
#include <Runtime/Base.hpp>
```

`Version` represent the version of one application, module or any version-controlled entity. Every version is composed by three numbers: `major`, `minor` and `patch`:

```c++
struct Version
{
	u32 major;
	u32 minor;
	u32 patch;
};
```

We suggest using the following rules to manage the version number:

1. An increment of `major` version indicates a breaking change to the interface of the entity, so that existing codes, programs and services using the entity must be explicitly modified to use the newer version of the entity correctly.
2. An increment of `minor` version indicates a non-breaking change to the interface of the entity, so that existing codes, programs and services can use the newer version of the entity correctly without any source-level modification.
3. An increment of `patch` version indicates a internal change of the entity and should not affect the entity interface, so that existing codes, programs and services can use the newer version of the entity correctly without any source-level modification.

## Pair and tuple types

```c++
#include <Runtime/Base.hpp> // For Pair.
#include <Runtime/Tuple.hpp> // For Tuple.
```

`Pair<T1, T2>` encapsulates one pair of elements with `T1` and `T2` type as the `first` and `second` element of the pair. `Pair` is mainly used by map containers to represent elements.

`Tuple<Tys...>` is a generalization of `Pair` and may contain one or multiple elements. Elements in `Tuple` can be fetched by calling `get<N>(tuple)` function. This type is mainly used to store function arguments in functional programming.