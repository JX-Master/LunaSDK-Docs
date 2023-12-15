# Luna::init

```c++
LUNA_RUNTIME_API bool init()
```

Initializes Luna SDK. 

Call this function to initialize Luna SDK. Most features provided by Luna SDK are only available after Luna SDK is initialized, so always initialize Luna SDK firstly on program startup. Calling this function when Luna SDK is already initialized does nothing and returns `true` directly.

Note that modules registered to Luna SDK will not be initialized by this function, they should be initialized manually using functions like init_modules. 

## Return value
Returns `true` if Luna SDK is succssfully initialized, returns `false` otherwise. 

