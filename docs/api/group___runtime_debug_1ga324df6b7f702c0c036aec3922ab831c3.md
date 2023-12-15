# Luna::stack_backtrace_symbols

```c++
LUNA_RUNTIME_API const c8 ** stack_backtrace_symbols(Span< const opaque_t > frames)
```

Gets symbolic names for frames returned by stack_backtrace. 



## Parameters
### frames
One buffer that contains frames to query. 

## Return value
Returns one array of strings that store symbolic names for frames. Strings are stored in the same order as `frames`. If the symbolic name of one frame is not found, `nullptr` will be written. 

#### Valid Usage


