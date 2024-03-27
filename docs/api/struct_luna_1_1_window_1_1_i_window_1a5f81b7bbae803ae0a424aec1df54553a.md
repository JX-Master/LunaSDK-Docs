# Luna::Window::IWindow::get_dpi_changed_event

```c++
virtual Event< window_dpi_changed_event_handler_t > & get_dpi_changed_event()=0
```

Gets the end dpi changed event of this window. 

This event will be emitted when the window DPI is changed. This may happen when the window is moved to another minitor with different DPI settings. 

## Return value
Returns one reference of the event object. 

