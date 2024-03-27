# Luna::Window::IWindow
Represents a system window that can be used to display user interface and can be drawn as surface. 

```c++
interface Luna::Window::IWindow : public virtual Interface
```

## Base type
* [Interface](struct_luna_1_1_interface.md)
## Member functions
* [virtual void close()=0](struct_luna_1_1_window_1_1_i_window_1af6ee7eacbde6b379b68d954e44f6e549.md)

    Closes this window. On single-window platforms, this causes the application to exit. 

* [virtual bool is_closed()=0](struct_luna_1_1_window_1_1_i_window_1ab389487cda294f9831ec97f51a8c1239.md)

    Checks whether the window is closed. The window handle is invalid when one window is closed. 

* [virtual bool is_focused()=0](struct_luna_1_1_window_1_1_i_window_1a638894f431c7b71bec6ea4f1e1ab611e.md)

    Checks whether the window has input focus. 

* [virtual RV set_focus()=0](struct_luna_1_1_window_1_1_i_window_1a90629685caf185a56d3d7014e0193149.md)

    Brings this window to front and acquires input focus for the window. 

* [virtual bool is_minimized()=0](struct_luna_1_1_window_1_1_i_window_1ade46e6ea5b89470a7ba1aff69f84b75c.md)

    Checks whether the window is minimized. 

* [virtual bool is_maximized()=0](struct_luna_1_1_window_1_1_i_window_1a2974797fb50bbdfe4e2f2593f60b32eb.md)

    Checks whether the window is maximized. 

* [virtual RV set_minimized()=0](struct_luna_1_1_window_1_1_i_window_1a5e18ae2fc2e78c6faa58158bff41b26c.md)

    Minimize the window. 

* [virtual RV set_maximized()=0](struct_luna_1_1_window_1_1_i_window_1a770823d0ec593012ed17ed00a30978e4.md)

    Maximize the window. 

* [virtual RV set_restored()=0](struct_luna_1_1_window_1_1_i_window_1aa10ee5f4d9171d0782ce08b0a1776b7a.md)

    Restore the window from minimized or maximized state. 

* [virtual bool is_hovered()=0](struct_luna_1_1_window_1_1_i_window_1a0780ed4e322b8db10129b2ddd7c6c466.md)

    Checks whether the cursor is currently directly over the content area of the window. 

* [virtual bool is_visible()=0](struct_luna_1_1_window_1_1_i_window_1aa8edf0d24fe5bde9fd8faf533326b250.md)

    Checks whether the window is visible. 

* [virtual RV set_visible(bool visible)=0](struct_luna_1_1_window_1_1_i_window_1a165469e3524d03378322d988719ccb72.md)

    Sets the visibility of the window. 

* [virtual bool is_resizable()=0](struct_luna_1_1_window_1_1_i_window_1acc722d4eaefdc679b06dc2c0a576afce.md)

    Checks whether the window is resizable by dragging the border of the window. 

* [virtual RV set_resizable(bool resizable)=0](struct_luna_1_1_window_1_1_i_window_1a398b2ae9b9d43a2354140be4f5fffaf2.md)

    Sets the resizable state of the window. 

* [virtual bool is_frameless()=0](struct_luna_1_1_window_1_1_i_window_1a579814f3685b3c9df436a67337062635.md)

    Checks whether the window is frameless. One frameless window does not have border, titlebar and close/minimize/maximize buttons. 

* [virtual RV set_frameless(bool frameless)=0](struct_luna_1_1_window_1_1_i_window_1ae98487512480fec45a23144a2348d6f4.md)

    Sets the frameless state of the window. 

* [virtual Int2U get_position()=0](struct_luna_1_1_window_1_1_i_window_1ad020ca1f0bf75e0c3767277c4bfd2cf1.md)

    Gets the position of the window client area. 

* [virtual RV set_position(i32 x, i32 y)=0](struct_luna_1_1_window_1_1_i_window_1a0bdb9f1aaa575f2e905c5add6bb0ce8f.md)

    Sets the position of the window client area. 

* [virtual UInt2U get_size()=0](struct_luna_1_1_window_1_1_i_window_1ac50b4bb5ecacd4f266f68f2894dc7502.md)

    Gets the size of the content area of the window measured in screen coordinates. 

* [virtual RV set_size(u32 width, u32 height)=0](struct_luna_1_1_window_1_1_i_window_1ab9110dcacc3ebd439497f877b453e78a.md)

    Sets the size of the content area of the window measured in screen coordinates. 

* [virtual UInt2U get_framebuffer_size()=0](struct_luna_1_1_window_1_1_i_window_1a7d1a3d760ad25aedb7ceb6f4a2545613.md)

    Gets the framebuffer size of the window context area in pixels. 

* [virtual f32 get_dpi_scale_factor()=0](struct_luna_1_1_window_1_1_i_window_1ae797fb280d215ff8868090e526c38fce.md)

    Gets the DPI scaling factor, which is the ratio between the current DPI and the platform's default DPI. 

* [virtual bool is_full_screen()=0](struct_luna_1_1_window_1_1_i_window_1a3e213171fe5e23d612b52ab4cd7d24e2.md)

    Checks whether the window is full screen. 

* [virtual monitor_t get_monitor()=0](struct_luna_1_1_window_1_1_i_window_1a3f197fe9169a6217d0bb6ef6d5b15eb0.md)

    Gets the monitor that one full screen window is attached to. Returns `nullptr` if the window is not in full-screen mode. 

* [virtual RV set_title(const c8 *title)=0](struct_luna_1_1_window_1_1_i_window_1a94b2449acbb8428d0cc80ec1d025b7f9.md)

    Sets the window title. 

* [virtual RV set_display_settings(const WindowDisplaySettings &display_settings)=0](struct_luna_1_1_window_1_1_i_window_1a25ccecb6822252934729664e253ccbc6.md)

    Sets the window display settings. 

* [virtual Int2U screen_to_client(const Int2U &point)=0](struct_luna_1_1_window_1_1_i_window_1aaf5b0070cfc3150e088e336ebe6698dc.md)

    Converts one screen coordinate to one client coordinate. 

* [virtual Int2U client_to_screen(const Int2U &point)=0](struct_luna_1_1_window_1_1_i_window_1a49f863c06b794dd2c5113c781955db48.md)

    Converts one client coordinate to one screen coordinate. 

* [virtual Event< window_close_event_handler_t > & get_close_event()=0](struct_luna_1_1_window_1_1_i_window_1a7ac867511ced89dbe23482e0ce6ea1ea.md)

    Gets the close event of this window. 

* [virtual Event< window_focus_event_handler_t > & get_focus_event()=0](struct_luna_1_1_window_1_1_i_window_1a1e493fd43ea77350e3df84dce6fa71f6.md)

    Gets the focus event of this window. 

* [virtual Event< window_lose_focus_event_handler_t > & get_lose_focus_event()=0](struct_luna_1_1_window_1_1_i_window_1aafaba799a84964425d67185148d5d8ed.md)

    Gets the lose focus event of this window. This event will be emitted when the window loses focus. 

* [virtual Event< window_show_event_handler_t > & get_show_event()=0](struct_luna_1_1_window_1_1_i_window_1a8550133fa01a9891ea3d8bd3ac78535c.md)

    Gets the show event of this window. 

* [virtual Event< window_hide_event_handler_t > & get_hide_event()=0](struct_luna_1_1_window_1_1_i_window_1a501108314e4878c64c73fe4af1f2d016.md)

    Gets the hide event of this window. 

* [virtual Event< window_resize_event_handler_t > & get_resize_event()=0](struct_luna_1_1_window_1_1_i_window_1a7c293102d28307cfc2ccfeda1d930277.md)

    Gets the resize event of this window. 

* [virtual Event< window_framebuffer_resize_event_handler_t > & get_framebuffer_resize_event()=0](struct_luna_1_1_window_1_1_i_window_1aa139c90488d0bf46e81725a4141c03f3.md)

    Gets the framebuffer resize event of this window. 

* [virtual Event< window_move_event_handler_t > & get_move_event()=0](struct_luna_1_1_window_1_1_i_window_1a8b64faecae9dc58137a76ace71b2dea7.md)

    Gets the move event of this window. 

* [virtual Event< window_begin_resize_move_t > & get_begin_resize_move_event()=0](struct_luna_1_1_window_1_1_i_window_1a007fd8ba54f7fbcf6082940ea4f4a457.md)

    Gets the begin resize move event of this window. 

* [virtual Event< window_end_resize_move_t > & get_end_resize_move_event()=0](struct_luna_1_1_window_1_1_i_window_1a897eaff9f8b5d88fcd2b0a574b4ba5e8.md)

    Gets the end resize move event of this window. 

* [virtual Event< window_dpi_changed_event_handler_t > & get_dpi_changed_event()=0](struct_luna_1_1_window_1_1_i_window_1a5f81b7bbae803ae0a424aec1df54553a.md)

    Gets the end dpi changed event of this window. 

* [virtual Event< window_key_down_event_handler_t > & get_key_down_event()=0](struct_luna_1_1_window_1_1_i_window_1ac611625fa262cfaf5e629189b4a2a83f.md)

    Gets the key down event of this window. 

* [virtual Event< window_key_up_event_handler_t > & get_key_up_event()=0](struct_luna_1_1_window_1_1_i_window_1aa9357873b6affee51e9a82df9e9958b9.md)

    Gets the key up event of this window. 

* [virtual Event< window_input_character_event_handler_t > & get_input_character_event()=0](struct_luna_1_1_window_1_1_i_window_1a279ff04af4c5748e44f520aa36ecee97.md)

    Gets the input character event of this window. 

* [virtual Event< window_mouse_move_event_handler_t > & get_mouse_move_event()=0](struct_luna_1_1_window_1_1_i_window_1a355ab3c7b8745603e2855d52f0556d0a.md)

    Gets the mouse move event of this window. 

* [virtual Event< window_mouse_down_event_handler_t > & get_mouse_down_event()=0](struct_luna_1_1_window_1_1_i_window_1ae685cc5edb080161393bc77919fe421d.md)

    Gets the mouse down event of this window. 

* [virtual Event< window_mouse_up_event_handler_t > & get_mouse_up_event()=0](struct_luna_1_1_window_1_1_i_window_1ac95afcc9b8632f97c54bba591774ce8e.md)

    Gets the mouse up event of this window. 

* [virtual Event< window_mouse_wheel_event_handler_t > & get_mouse_wheel_event()=0](struct_luna_1_1_window_1_1_i_window_1a568577c55a5b8b589f1a776d8228bf7f.md)

    Gets the mouse wheel event of this window. 

* [virtual Event< window_touch_event_handler_t > & get_touch_event()=0](struct_luna_1_1_window_1_1_i_window_1aa0936cdc0b127997c58291e0477971a6.md)

    Gets the touch event of this window. 

* [virtual Event< window_drop_file_event_handler_t > & get_drop_file_event()=0](struct_luna_1_1_window_1_1_i_window_1a5174d0c15f91591c09ed85c0d84e05c8.md)

    Gets the drop file event of this window. 

