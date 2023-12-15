# Luna::Path::remove_extension

```c++
void remove_extension()
```

Removes the extension. 

## Overview
The extension separator (".") is removed as well in this operation. If the path does not have one extension (`extension().empty() == true`), this operation does nothing. 

