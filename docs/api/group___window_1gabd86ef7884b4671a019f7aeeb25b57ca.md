# Luna::Window::open_dir_dialog

```c++
R< Path > open_dir_dialog(const c8 *title=nullptr, const Path &initial_dir=Path())
```

Displays one open directory dialog and fetches the selecting results. 



## Parameters
* *in* **title**

    The title of the dialog, encoded in UTF-8. If this is `nullptr`, the platform-specific default title will be used. 

* *in* **initial_dir**

    The initial directory to set the file dialog to. If this is empty, the system decides the default directory. This path must be a platform native path if specified. 

## Return value
Returns the user-specified directory path. The path is platform native, absolute path. 

## Valid Usage
* If `title` is not `nullptr`, `title` must specify one null-terminated string. 

