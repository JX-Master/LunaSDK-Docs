# Luna::Window::IWindow::get_hide_event

```c++
virtual Event< window_hide_event_handler_t > & get_hide_event()=0
```

Gets the hide event of this window. 

This event will be emitted when the window is completly hidden from the user. The client code should stop receiving inputs from the window and stop rendering to the window after receiving this event. 

## Return value
Returns one reference of the event object. 

