# HID
Human [Interface](struct_luna_1_1_interface.md) Device (HID) module provides APIs to access platform's input and output devices, like mouse, keyboard, controller, etc. 

## Types
* [Luna::HID::ControllerInputState](struct_luna_1_1_h_i_d_1_1_controller_input_state.md)

    The fetched input state for one generic game controller. 


* [Luna::HID::ControllerOutputState](struct_luna_1_1_h_i_d_1_1_controller_output_state.md)

    The state to set for a controller. 


## Enumerations
* [Luna::HID::ControllerButton](group___h_i_d_1ga436467ac9bceac9ecfbd3775068d34da.md)

    Specifies controller buttons. These values can be bitwise-OR combined to select multiple mouse buttons if needed. 

* [Luna::HID::KeyCode](group___h_i_d_1ga912f74cfa86bfd7af0ee6bb9010eba51.md)

    A platform-independent key code mapping for standard QWERTY keyboard. 

* [Luna::HID::MouseButton](group___h_i_d_1ga7823b2b124c60f1e08e41e482daddbb3.md)

    Specifies mouse button. These values can be bitwise-OR combined to select multiple mouse buttons if needed. 

## Functions
* [bool supports_controller()](group___h_i_d_1gad3ca103bf79091dbaec83d6a35c44fe6.md)

    Checks if game controller input is supported on the current platform. 

* [ControllerInputState get_controller_state(u32 index)](group___h_i_d_1gaf0ef8b9c177325759f937b0a82176bb3.md)

    Fetches the input state of the specified controller. 

* [RV set_controller_state(u32 index, const ControllerOutputState &state)](group___h_i_d_1ga11f141e5db38ab23f0f483145486f27d.md)

    Sets the output state of the specified controller. 

* [bool supports_keyboard()](group___h_i_d_1ga8190f504bfec80e16cdcb6f1d3d65cbd.md)

    Checks if keyboard input is supported on the current platform. 

* [bool get_key_state(KeyCode key)](group___h_i_d_1gaaae6c513317a33237154fc8718dba63a.md)

    Checks the if the specified key on the keyboard is pressed. 

* [bool supports_mouse()](group___h_i_d_1ga9a3ae36dee968577e16ebc458f659f84.md)

    Checks if mouse input is supported on the current platform. 

* [bool get_mouse_button_state(MouseButton mouse_button)](group___h_i_d_1ga5898fe9c725effba90892ec48e782ac3.md)

    Checks if the specified mouse button is pressed. 

* [Int2U get_mouse_pos()](group___h_i_d_1gaa54156da0fd14f9776a5efc78c3dbbfc.md)

    Get the position of the mouse cursor in screen space. 

* [RV set_mouse_pos(i32 x, i32 y)](group___h_i_d_1gac7e975e34d1d3b696c184fa35a24e535.md)

    Sets the OS mouse cursor position. The position is based on the screen coordinates. This only works for platforms that support mouse input. 

