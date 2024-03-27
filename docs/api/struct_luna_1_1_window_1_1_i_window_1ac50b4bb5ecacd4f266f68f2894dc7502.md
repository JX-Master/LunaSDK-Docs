# Luna::Window::IWindow::get_size

```c++
virtual UInt2U get_size()=0
```

Gets the size of the content area of the window measured in screen coordinates. 



## Remark
The screen coordinates is not necessary measured in pixels. For pixel-related operations, use `get_framebuffer_size` instead. 

