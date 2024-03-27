# Luna::Window::open_file_dialog

```c++
R< Vector< Path > > open_file_dialog(const c8 *title=nullptr, Span< const FileDialogFilter > filters={}, const Path &initial_dir=Path(), FileDialogFlag flags=FileDialogFlag::none)
```

Displays one open file dialog and fetches the selecting results. 



## Parameters
* *in* **title**

    The title of the dialog, encoded in UTF-8. If this is `nullptr`, the platform-specific default title will be used. 

* *in* **filters**

    The filters used by the open file dialog. If this is empty, the user can select any file types. 

* *in* **initial_dir**

    The initial directory to set the file dialog to. If this is empty, the system decides the default directory. This path must be a platform native path if specified. 

* *in* **flags**

    The additional flags. 

## Return value
Returns a list of selected file paths. All paths are platform native, absolute paths. 

## Valid Usage
* If `title` is not `nullptr`, `title` must specify one null-terminated string. 

