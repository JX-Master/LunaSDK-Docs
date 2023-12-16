# Luna::stack_backtrace_symbols

```c++
const c8 ** stack_backtrace_symbols(Span< const opaque_t > frames)
```

Gets symbolic names for frames returned by [stack_backtrace](group___runtime_debug_1gacf9a33547a6d81bec8edfb2e23ffd020.md). 



## Parameters
### frames
One buffer that contains frames to query. 

## Return value
Returns one array of strings that store symbolic names for frames. Strings are stored in the same order as `frames`. If the symbolic name of one frame is not found, `nullptr` will be written. 

## Valid Usage
1. All frames in `frames` must be valid frames returned by [stack_backtrace](group___runtime_debug_1gacf9a33547a6d81bec8edfb2e23ffd020.md). In particular, if the return value of [stack_backtrace](group___runtime_debug_1gacf9a33547a6d81bec8edfb2e23ffd020.md) is smaller than the size of the frame buffer passed to [stack_backtrace](group___runtime_debug_1gacf9a33547a6d81bec8edfb2e23ffd020.md), only valid frames, not the whole buffer, shall be specified in this call. 

