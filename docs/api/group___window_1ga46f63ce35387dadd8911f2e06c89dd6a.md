# Luna::Window::window_touch_event_handler_t

```c++
using window_touch_event_handler_t =  void(IWindow* window, Span<WindowEventTouchPoint> touches, u32 changed_mask)
```

The handler for touch event. 



## Parameters
* *in* **touches**

    The span that includes all touch points for this event. 

* *in* **changed_mask**

    A bit-combined mask to identify whether every touch point is changed between multiple touch events. Use `(changed_mask & (1 << i))` to test the touch point `i`, where `i` is the index of `touches`. 

