# Luna::FileOpenFlag

```c++
enum FileOpenFlag : u32
{
    read= 0x01
    write= 0x02
    user_buffering= 0x04
}
```

Specifies attributes for one file open operation. 

## Options
* [read](group___runtime_file_1ggaa6e577ca0057e9e199efe810f7876d3daecae13117d6f0584c25a9da6c8f8415e.md)

    Grants read access to the file so that [IFile::read](struct_luna_1_1_i_stream_1a6a5956c629eb0bba95dc0dd89bd0abde.md) operations can be performed. 

* [write](group___runtime_file_1ggaa6e577ca0057e9e199efe810f7876d3daefb2a684e4afb7d55e6147fbe5a332ee.md)

    Grants write access to the file so that [IFile::write](struct_luna_1_1_i_stream_1ae2de26864471bdff2d8f7d49ac47da39.md) operations can be performed. 

* [user_buffering](group___runtime_file_1ggaa6e577ca0057e9e199efe810f7876d3daef378d24dd8957b844c64cab7f2ae7ab.md)
