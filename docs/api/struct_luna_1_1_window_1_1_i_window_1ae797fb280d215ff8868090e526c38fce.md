# Luna::Window::IWindow::get_dpi_scale_factor

```c++
virtual f32 get_dpi_scale_factor()=0
```

Gets the DPI scaling factor, which is the ratio between the current DPI and the platform's default DPI. 



## Return value
Returns the DPI scaling factor. The default (unscaled) DPI factor is 1.0. 

## Remark
The DPI scale factor may be used if DPI scaling is enabled on the target monitor. 

