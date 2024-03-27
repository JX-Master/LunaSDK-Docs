# Luna::Window::IGLFWWindow
Implemented by the window object if the underlying window is a GLFW window. This interface is enabled on Windows, Linux and macOS platform. 

```c++
interface Luna::Window::IGLFWWindow : public virtual IWindow
```

## Base type
* [IWindow](struct_luna_1_1_window_1_1_i_window.md)
## Member functions
* [virtual GLFWwindow * get_glfw_window_handle()=0](struct_luna_1_1_window_1_1_i_g_l_f_w_window_1af5bb839cd6a47d65b4369f3ddad2cef1.md)

    Gets GLFWwindow* handle of this window. 

