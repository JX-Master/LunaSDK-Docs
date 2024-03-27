# Window
The Window module provides window management functionalities of the underlying system. 

## Types
* [Luna::Window::StartupParams](struct_luna_1_1_window_1_1_startup_params.md)

    Platform-specific application startup parameters. 


* [Luna::Window::ICocoaWindow](struct_luna_1_1_window_1_1_i_cocoa_window.md)

    Implemented by window object on macOS platform. 


* [Luna::Window::FileDialogFilter](struct_luna_1_1_window_1_1_file_dialog_filter.md)

    Specifies one filter that allows the user to filter files with specified types in file dialogs. 


* [Luna::Window::IGLFWWindow](struct_luna_1_1_window_1_1_i_g_l_f_w_window.md)

    Implemented by the window object if the underlying window is a GLFW window. This interface is enabled on Windows, Linux and macOS platform. 


* [Luna::Window::VideoMode](struct_luna_1_1_window_1_1_video_mode.md)

    Describes one video mode of one monitor. 


* [Luna::Window::WindowEventTouchPoint](struct_luna_1_1_window_1_1_window_event_touch_point.md)

    Identifies one touch point in one window touch event. 


* [Luna::Window::WindowDisplaySettings](struct_luna_1_1_window_1_1_window_display_settings.md)

    The window display settings. 


* [Luna::Window::IWindow](struct_luna_1_1_window_1_1_i_window.md)

    Represents a system window that can be used to display user interface and can be drawn as surface. 


* [Luna::Window::IWin32Window](struct_luna_1_1_window_1_1_i_win32_window.md)

    Implemented by window object on Windows platform. 


## Enumerations
* [Luna::Window::FileDialogFlag](group___window_1ga18929cfa2095b72149810a1e01fb6071.md)

    The flags for opening one file dialog. 

* [Luna::Window::MessageBoxType](group___window_1gadd59b374906c25417d6593d866c81616.md)

    Specifies the type of the message box. 

* [Luna::Window::MessageBoxIcon](group___window_1gadb20e219f0280feb82aee8f32761bcb3.md)

    Specifies the icon that will be displayed on the message box. 

* [Luna::Window::MessageBoxButton](group___window_1ga3b060141e4128fc1c2dd75873f6adafb.md)

    Indicates buttons on the message box. 

* [Luna::Window::ModifierKeyFlag](group___window_1gaa11a96e38e6dbe42e4bc553ed7cfac42.md)

    Identifies keys that are pressed in window mouse events. 

* [Luna::Window::WindowCreationFlag](group___window_1ga2d312ae999122d8a4b957464d0b03ab1.md)

    Flags that specifies the initial state and style of the window. 

## Alias types
* [using monitor_t =  opaque_t](group___window_1ga43a9d174a0de96a1eb81257b2f87a0cb.md)

    The opaque handle that represents the system moditor. 

* [using window_close_event_handler_t =  void(IWindow* window)](group___window_1gadac4f21829cc8dd970fb10723277b3ec.md)

    The hanlder for window close event. 

* [using window_focus_event_handler_t =  void(IWindow* window)](group___window_1ga5c8c2846f1f4b4ffa5bfb5e2a4129883.md)

    The handler for window focus event. 

* [using window_lose_focus_event_handler_t =  void(IWindow* window)](group___window_1ga03407e3d43e44a7c875f87677e65c7e6.md)

    The handler for window lose foucs event. 

* [using window_show_event_handler_t =  void(IWindow* window)](group___window_1ga9dde089590d3f9fd06f2dbddd69e3b31.md)

    The handler for window show event. 

* [using window_hide_event_handler_t =  void(IWindow* window)](group___window_1ga41fbfea642c1d061688247ba2ad00ce3.md)

    The handler for window hide event. 

* [using window_resize_event_handler_t =  void(IWindow* window, u32 width, u32 height)](group___window_1gadf30a785fc5c4b13046ee2dcccaeda93.md)

    The handler for window resize event. 

* [using window_framebuffer_resize_event_handler_t =  void(IWindow* window, u32 width, u32 height)](group___window_1ga2350f99a7862ff459fa511d79281df23.md)

    The handler for window framebuffer resize event. 

* [using window_move_event_handler_t =  void(IWindow* window, i32 x, i32 y)](group___window_1ga4e020464c9332cb8dec8a2772a678d79.md)

    The handler for window move resize event. 

* [using window_begin_resize_move_t =  void(IWindow* window)](group___window_1ga851e0e411b5e14c8be8b4819b3a0022c.md)

    The handler for window begin resize move event. 

* [using window_end_resize_move_t =  void(IWindow* window)](group___window_1ga10016c5807e46009b5b2d924d50cee5e.md)

    The handler for window end resize move event. 

* [using window_dpi_changed_event_handler_t =  void(IWindow* window, f32 dpi_scale)](group___window_1ga7a214979e471171f143c3e13fab5f595.md)

    The handler for window dpi changed event. 

* [using window_key_down_event_handler_t =  void(IWindow* window, HID::KeyCode key)](group___window_1ga8aa428fe6ddb6cb9828b98f6a4529d31.md)

    The handler for window key down event. 

* [using window_key_up_event_handler_t =  void(IWindow* window, HID::KeyCode key)](group___window_1gaa6a45aa3eda812f08d0a3b7b9d01aa44.md)

    The handler for window key up event. 

* [using window_input_character_event_handler_t =  void(IWindow* window, c32 character)](group___window_1gaa4386f8af3351a1e2332ed2471d83776.md)

    The handler for window input character event. 

* [using window_mouse_move_event_handler_t =  void(IWindow* window, i32 x, i32 y)](group___window_1ga9cd6fe6925f5ae24acdf6fee018412ef.md)

    The handler for mouse move event. 

* [using window_mouse_down_event_handler_t =  void(IWindow* window, ModifierKeyFlag modifier_flags, HID::MouseButton button)](group___window_1gaa0c870690863db174474ded9f57bb3e6.md)

    The handler for mouse down event. 

* [using window_mouse_up_event_handler_t =  void(IWindow* window, ModifierKeyFlag modifier_flags, HID::MouseButton button)](group___window_1ga05954dc7646e054549249fbce3fc287b.md)

    The handler for mouse up event. 

* [using window_mouse_wheel_event_handler_t =  void(IWindow* window, f32 x_wheel_delta, f32 y_wheel_delta)](group___window_1ga233650a21057c05de6b8c8877311e5ac.md)

    The handler for mouse up event. 

* [using window_touch_event_handler_t =  void(IWindow* window, Span<WindowEventTouchPoint> touches, u32 changed_mask)](group___window_1ga46f63ce35387dadd8911f2e06c89dd6a.md)

    The handler for touch event. 

* [using window_drop_file_event_handler_t =  void(IWindow* window, i32 x, i32 y, Span<const c8*> paths)](group___window_1ga5b1bd1739e0c545fa8f6db526c7bfd6f.md)

    The handler for drop file event. 

## Constants
* [constexpr i32 DEFAULT_POS](group___window_1ga215ec580a3acb85974aebe2346066319.md)

    Specify this value as `x` or `y` of the window to let windowing system choose one suitable position for the window. 

## Functions
* [void set_startup_params(const StartupParams &params)](group___window_1ga8b673b742e7dd97fdbe78d9cb04ec7d6.md)

    Sets the startup parameters for Window module. This should be called before the Window module is initialized. 

* [const c8 * get_name()](group___window_1ga746b4ca92eaba2141155d20a3a5598d3.md)

    Gets the application name. 

* [Version get_version()](group___window_1ga4f3381927b1dca5eb9a421a703b2b3de.md)

    Gets the application version. 

* [R< Vector< Path > > open_file_dialog(const c8 *title=nullptr, Span< const FileDialogFilter > filters={}, const Path &initial_dir=Path(), FileDialogFlag flags=FileDialogFlag::none)](group___window_1ga090a80d0fbe050bb81bae074bea0c869.md)

    Displays one open file dialog and fetches the selecting results. 

* [R< Path > save_file_dialog(const c8 *title=nullptr, Span< const FileDialogFilter > filters={}, const Path &initial_file_path=Path(), FileDialogFlag flags=FileDialogFlag::none)](group___window_1gad8f4c7a59e964d2292892c0040bc2573.md)

    Displays one save file dialog and fetches the selecting results. 

* [R< Path > open_dir_dialog(const c8 *title=nullptr, const Path &initial_dir=Path())](group___window_1gabd86ef7884b4671a019f7aeeb25b57ca.md)

    Displays one open directory dialog and fetches the selecting results. 

* [R< MessageBoxButton > message_box(const c8 *text, const c8 *caption, MessageBoxType type, MessageBoxIcon icon=MessageBoxIcon::none)](group___window_1ga1561c4a2f9c6fceb36509508ad70d9ef.md)

    Displays one message box dialog. The current thread blocks until the dialog is closed. 

* [monitor_t get_primary_monitor()](group___window_1ga1f839e1d9f501c7758a3616b9f5ccbe6.md)

    Gets the primary monitor of the platform. 

* [u32 count_monitors()](group___window_1ga0d8fbc07bc9158ae66544f8300920774.md)

    Gets the number of monitors currently connected to the platform. 

* [monitor_t get_monitor(u32 index)](group___window_1gacdf6958dec866ccf5c7df89218c8ee0f.md)

    Gets the monitor at specified index. 

* [Event< monitor_event_handler_t > & get_monitor_event()](group___window_1ga952c81b35afd1b7dc6b096fb4f48972e.md)

    Gets the event that will be called when one monitor event is triggered. 

* [u32 count_monitor_supported_video_modes(monitor_t monitor)](group___window_1ga2136c2eac4de94a302e07a8e7c1fed74.md)

    Gets the number of supported video modes of the monitor. 

* [VideoMode get_monitor_supported_video_mode(monitor_t monitor, u32 index)](group___window_1gafbdcb042a8c6306c06edb863ffc7fc52.md)

    Gets the supported video mode of the monitor at the specified index. 

* [VideoMode get_monitor_video_mode(monitor_t monitor)](group___window_1gafc014148e1478ccedc34d5051b6e6a01.md)

    Gets the current video mode of the monitor. 

* [UInt2U get_monitor_physical_size(monitor_t monitor)](group___window_1ga4f88a3e6ec77f63c05d0c4f0e44b2bd6.md)

    Gets the physical size of the monitor measured in millimetres. 

* [f32 get_monitor_dpi_scale_factor(monitor_t monitor)](group___window_1ga1984e0a5c8f6c650077bea59b8d1e2d2.md)

    Gets the DPI scale factor of the monitor. 

* [Int2U get_monitor_position(monitor_t monitor)](group___window_1ga86421a2da63104db91833b64598b694f.md)

    Gets the virtual position of the monitor in screen coordinates. 

* [RectI get_monitor_working_area(monitor_t monitor)](group___window_1ga6d8415dfb9677df2ccb15e1ecf6584a4.md)

    Gets the working area of the monitor, that is, the area not occupied by the system UI like taskbars or menu bars. 

* [Name get_monitor_name(monitor_t monitor)](group___window_1ga7f5201997eb7d2e0ebbddb8672ae6bff.md)

    Gets the name of the monitor. 

* [R< VkSurfaceKHR > new_vulkan_surface_from_window(VkInstance instance, IWindow *window)](group___window_1ga8535f2645ff7b1d33e6fa47aa497c4e2.md)

    Creates a vulkan surface form window. 

* [Span< const c8 * > get_required_vulkan_instance_extensions()](group___window_1gadd36facc6a621e9ace90240b7831cc16.md)

    Gets an array of vulkan instance extensions required by the window module to create vulkan surface from [IWindow](struct_luna_1_1_window_1_1_i_window.md). 

* [void poll_events(bool wait_events=false)](group___window_1gad0dfe33dedf083f8016ca0b5d49ba254.md)

    Processes window events for all windows created from the current thread. 

* [R< Ref< IWindow > > new_window(const c8 *title, const WindowDisplaySettings &display_settings, WindowCreationFlag flags=WindowCreationFlag::none)](group___window_1ga1042e96643074be4e6cf4b87c5955f4e.md)

    Creates one new window. The new window will be displayed immediately unless [WindowCreationFlag::hidden](group___window_1gga2d312ae999122d8a4b957464d0b03ab1a662f707d5491e9bce8238a6c0be92190.md) is set. 

