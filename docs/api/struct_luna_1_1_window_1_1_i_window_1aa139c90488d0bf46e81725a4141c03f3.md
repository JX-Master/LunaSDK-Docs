# Luna::Window::IWindow::get_framebuffer_resize_event

```c++
virtual Event< window_framebuffer_resize_event_handler_t > & get_framebuffer_resize_event()=0
```

Gets the framebuffer resize event of this window. 

This event will be emitted when the window's framebuffer size is changed. 

## Return value
Returns one reference of the event object. 

