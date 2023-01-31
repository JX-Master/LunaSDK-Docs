# Initialization and Shutdown

## SDK Initialization

```c++
#include <Runtime/Runtime.hpp>
```

Call `Luna::init` to initialize Luna SDK. Most features provided by Luna SDK are only available after Luna SDK is initialized, so always initialize Luna SDK firstly on program startup. `Luna::init` returns one `bool` value, which indicates whether the initialization is succeeded. After the initialization is succeeded, following calls to `Luna::init` does nothing and returns `true` directly.

Note that modules registered to Luna SDK will not be initialized by `Luna::init`, they should be initialized manually using functions like `init_modules`. See [Module Management](module_management.md) for details.

## SDK shutdown

```c++
#include <Runtime/Runtime.hpp>
```

Call `Luna::close` to close Luna SDK. Most features provided by Luna SDK are not available after Luna SDK is closed. If Luna SDK is already closed, calling `Luna::close` does nothing and returns directly.

Unlike SDK initialization, initialized modules **will** be closed by `Luna::close` in the reverse order of their initialization order, so they don't need to be closed manually.

### Release resources before closing SDK

All dynamic memory allocated from `memalloc`, `memrealloc` and `memnew` must be freed before calling `Luna::close`. All boxed object created from `new_object` and `object_alloc` must be released before calling `Luna::close`. Calls to `memfree`, `memdelete`, `object_release` and other functions after `Luna::close` results in undefined behavior, and usually a program crash. This often happens when you declare global variables that hold dynamic allocated resources (such as `Ref`) and memory blocks (such as `UniquePtr`, and containers like `Vector`, `HashMap`, etc.). Remember to clear such resources before calling `Luna::close`. For some containers, you should call `clear` then `shrink_to_fit` to eventually frees the internal memory buffer used by containers.





