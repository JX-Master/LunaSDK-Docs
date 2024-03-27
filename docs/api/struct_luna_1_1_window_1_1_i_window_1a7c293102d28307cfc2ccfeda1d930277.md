# Luna::Window::IWindow::get_resize_event

```c++
virtual Event< window_resize_event_handler_t > & get_resize_event()=0
```

Gets the resize event of this window. 

This event will be emitted when the window size is changed. The new size may be 0 if the window is minimized. 

## Return value
Returns one reference of the event object. 

