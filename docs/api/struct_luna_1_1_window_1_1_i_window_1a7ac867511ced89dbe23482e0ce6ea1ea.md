# Luna::Window::IWindow::get_close_event

```c++
virtual Event< window_close_event_handler_t > & get_close_event()=0
```

Gets the close event of this window. 

Usually the user should close the window by calling [IWindow::close](struct_luna_1_1_window_1_1_i_window_1af6ee7eacbde6b379b68d954e44f6e549.md) to respond this event. This event will be emitted when the close button of the window is pressed. 

## Return value
Returns one reference of the event object. 

