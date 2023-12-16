# lutry

```c++
#define lutry
```

Opens one try block that encapsulates expressions that may fail. 



## Valid Usage
* Every function body can have only one try-catch block that encapsulates all expressions that may fail. If you need multiple try-catch blocks, you can use dedicated functions to wrap each try-catch block, then call such functions in your original function. 

