# Luna::HID::ControllerInputState
The fetched input state for one generic game controller. 

```c++
struct Luna::HID::ControllerInputState
```

## Member objects
* [bool connected](struct_luna_1_1_h_i_d_1_1_controller_input_state_1ab36823025f12a809217f7771125658c2.md)

    Whether this device is connected and the state is valid. 

* [ControllerButton buttons](struct_luna_1_1_h_i_d_1_1_controller_input_state_1a73754ea6de21a25d84d0ba24a5a35869.md)

    A combination of bits to represent the pressed state of each button (1 for pressed, 0 for not pressed). 

* [f32 axis_lx](struct_luna_1_1_h_i_d_1_1_controller_input_state_1af717a1deeecad99e882d49e0b18115b5.md)

    The x axis for left pad, mapped to [-1, 1]. 

* [f32 axis_ly](struct_luna_1_1_h_i_d_1_1_controller_input_state_1ad6f994eb1c0560ee407c567b108c717a.md)

    The y axis for left pad, mapped to [-1, 1]. 

* [f32 axis_rx](struct_luna_1_1_h_i_d_1_1_controller_input_state_1a28914c1cb9d4aae0135f3aa09eeb7614.md)

    The x axis for right pad, mapped to [-1, 1]. 

* [f32 axis_ry](struct_luna_1_1_h_i_d_1_1_controller_input_state_1acfe37614e8933cd923d3790541b9464b.md)

    The y axis for right pad, mapped to [-1, 1]. 

* [f32 axis_lt](struct_luna_1_1_h_i_d_1_1_controller_input_state_1a54bdf2e05c572a60ac46f927dc163ae8.md)

    The left trigger value, mapped to [0, 1]. For non-linear controllers, the value is either 0 or 1. [ControllerButton::lt](group___h_i_d_1gga436467ac9bceac9ecfbd3775068d34daad91af6958918af87d6a057c1cdf5b225.md) is also set if this value is greater one system-specified threshold. 

* [f32 axis_rt](struct_luna_1_1_h_i_d_1_1_controller_input_state_1aef180acb766caf93eb2fdc73ca47686a.md)

    The right trigger value, mapped to [0, 1]. For non-linear controllers, the value is either 0 or 1. [ControllerButton::rt](group___h_i_d_1gga436467ac9bceac9ecfbd3775068d34daa822050d9ae3c47f54bee71b85fce1487.md) is also set if this value is greater one system-specified threshold. 

