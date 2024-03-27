# Luna::Window::WindowDisplaySettings::monitor

```c++
monitor_t monitor
```

The monitor that displays the window. 

On full screen mode, if this is `nullptr`, window will be displayed on the main monitor.

This must be `nullptr` if `full_screen` is `false`. 

