# Luna::Window::IWindow::get_show_event

```c++
virtual Event< window_show_event_handler_t > & get_show_event()=0
```

Gets the show event of this window. 

This event will be emitted when the window is visible to the user. The client code should continue receiving inputs from the window and continue rendering to the window after receiving this event. 

## Return value
Returns one reference of the event object. 

