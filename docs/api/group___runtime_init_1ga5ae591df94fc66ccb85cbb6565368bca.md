# Luna::close

```c++
void close()
```

Closes Luna SDK. 

Call this function to close Luna SDK. Most features provided by Luna SDK are not available after Luna SDK is closed. Calling this function when Luna SDK is not initialized or already closed does nothing and returns directly.

Initialized modules *will* be closed by this function in the reverse order of their initialization order, so they don't need to be closed manually. 

## Remark
All dynamic memory allocated from [memalloc](group___runtime_memory_1ga341bf6dd4a6ca9712174e6548774bc31.md), [memrealloc](group___runtime_memory_1ga9e2c0a02d9b513dc3f7f1b101860d11f.md) and [memnew](group___runtime_memory_1ga81e30b31f5e8a02f54478a634015e720.md) must be freed before calling [close](group___runtime_init_1ga5ae591df94fc66ccb85cbb6565368bca.md), all boxed objects created from [new_object](group___runtime_1gaa7e539a91bc5a8e68c91db8d2d8a9c23.md) and [object_alloc](group___runtime_object_1gabbcaac45f20e9e4c322fb1db0376b641.md) must be released before calling [close](group___runtime_init_1ga5ae591df94fc66ccb85cbb6565368bca.md) too. Calls to [memfree](group___runtime_memory_1ga102bf0df13784b9f636c555461862a14.md), [memdelete](group___runtime_memory_1gaf95818ee40a0536baee3f539b019df5d.md), [object_release](group___runtime_object_1ga7f822bf9876967630b4090507fff9465.md) and other functions after [close](group___runtime_init_1ga5ae591df94fc66ccb85cbb6565368bca.md) results in undefined behavior, and usually a program crash. This often happens when you declare global variables that hold dynamic allocated resources (such as [Ref](class_luna_1_1_ref.md)) and memory blocks (such as [UniquePtr](class_luna_1_1_unique_ptr.md), and containers like [Vector](class_luna_1_1_vector.md), [HashMap](class_luna_1_1_hash_map.md), etc.). Remember to clear such resources before calling [close](group___runtime_init_1ga5ae591df94fc66ccb85cbb6565368bca.md). For some containers, you should call `clear` then `shrink_to_fit` to eventually frees the internal memory buffer used by containers. 

