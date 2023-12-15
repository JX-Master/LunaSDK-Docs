# Luna::ModuleDesc::dependencies

```c++
const c8* dependencies
```

A string that records modules this module depends on. 

## Overview
the lifetime of the module.

In case that multiple modules are required, use semicolons(;) to separate them (for example: "Core;Input;Gfx"). There should not be any semicolon after the last item in the string.

Dependencies to `Runtime` should not be listed here. The Runtime is always initialized before any other module gets initialized. 

