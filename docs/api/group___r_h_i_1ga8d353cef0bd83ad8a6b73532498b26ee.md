# Luna::RHI::LoadOp

```c++
enum LoadOp : u8
{
    dont_care= 0
    load= 1
    clear= 2
}
```

The operation to perform when the attachment is loaded to GPU. 

## Options
* [dont_care](group___r_h_i_1gga8d353cef0bd83ad8a6b73532498b26eeabe7bbe0cf3947e795861f1fa966bab58.md)

    The previous contents of the attachment does not need to be preserved. If this is specified, your application should not have any assumptions on the initial data of the attachment, and should overwrite the data in render pass. 

* [load](group___r_h_i_1gga8d353cef0bd83ad8a6b73532498b26eeaec4d1eb36b22d19728e9d1d23ca84d1c.md)

    The previous contents of the attachment shall be preserved. 

* [clear](group___r_h_i_1gga8d353cef0bd83ad8a6b73532498b26eea01bc6f8efa4202821e95f4fdf6298b30.md)

    The contents within of the attachment will be cleared to a uniform value. 

