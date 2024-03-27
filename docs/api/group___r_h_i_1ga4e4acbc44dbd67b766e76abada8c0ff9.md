# Luna::RHI::TextureViewType

```c++
enum TextureViewType : u8
{
    unspecified= 0
    tex1d
    tex2d
    tex2dms
    tex3d
    texcube
    tex1darray
    tex2darray
    tex2dmsarray
    texcubearray
}
```

Specifies the texture view type, which is how render pipeline interprets texture data. 

## Options
* [unspecified](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9ad415f0e30c471dfdd9bc4f827329ef48.md)

    Uses the texture resource's type as the texture view type. 

* [tex1d](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a2be0dbf8f8b01dfb26ff8c464caad189.md)

    Interprets texture data as one 1D texture. 

* [tex2d](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a68d62dd2c0dea0a7386e98c6d9e95a1e.md)

    Interprets texture data as one 2D texture. 

* [tex2dms](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a2714d280697d6b3968190c29f63bb831.md)

    Interprets texture data as one 2D multi-sample texture. 

* [tex3d](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a46435dfdd61fe1af7248de1e8751b1cd.md)

    Interprets texture data as one 3D texture. 

* [texcube](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a3fa65c7dfa951f175afde47b54ba997a.md)

    Interprets texture data as one cube texture. 

* [tex1darray](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a1afe04debd1227b26d7a71144e4241f2.md)

    Interprets texture data as one 1D texture array. 

* [tex2darray](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a700fcd8bf38e4aeb2e93a900b41c5ae8.md)

    Interprets texture data as one 2D texture array. 

* [tex2dmsarray](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9aac18bbd1aacd895c31e4175318ec5502.md)

    Interprets texture data as one 2D multi-sample texture array. 

* [texcubearray](group___r_h_i_1gga4e4acbc44dbd67b766e76abada8c0ff9a5b35911622429c30feda25457f827a4e.md)

    Interprets texture data as one cube texture array. 

