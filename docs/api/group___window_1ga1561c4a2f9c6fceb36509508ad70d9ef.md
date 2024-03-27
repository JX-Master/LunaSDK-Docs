# Luna::Window::message_box

```c++
R< MessageBoxButton > message_box(const c8 *text, const c8 *caption, MessageBoxType type, MessageBoxIcon icon=MessageBoxIcon::none)
```

Displays one message box dialog. The current thread blocks until the dialog is closed. 



## Parameters
* *in* **text**

    The UTF-8 text that will be displayed in the message box. 

* *in* **caption**

    The caption (title) of the message box. 

* *in* **type**

    The type of the message box, 

* *in* **icon**

    The icon of the message box. Default value is [MessageBoxIcon::none](group___window_1ggadb20e219f0280feb82aee8f32761bcb3a334c4a4c42fdb79d7ebc3e73b517e6f8.md), which does not show any icon. 

## Return value
Returns the button clicked by the user. 

## Valid Usage
* `text` and `caption` must specify null-terminated strings. 

