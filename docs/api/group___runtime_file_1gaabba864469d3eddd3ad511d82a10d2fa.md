# Luna::FileAttributeFlag

```c++
enum FileAttributeFlag : u32
{
    read_only= 0x01
    hidden= 0x02
    directory= 0x04
    character_special= 0x08
    block_special= 0x10
}
```

Represents file binary attributes. 

## Options
* [read_only](group___runtime_file_1ggaabba864469d3eddd3ad511d82a10d2faabefe72871b2de8f4f0e20108517e31fe.md)

    This file is a read-only file. One read-only directory denotes a read-only file system. 

* [hidden](group___runtime_file_1ggaabba864469d3eddd3ad511d82a10d2faa662f707d5491e9bce8238a6c0be92190.md)

    This file is a hidden file. 

* [directory](group___runtime_file_1ggaabba864469d3eddd3ad511d82a10d2faa5f8f22b8cdbaeee8cf857673a9b6ba20.md)

    This file is a directory. 

* [character_special](group___runtime_file_1ggaabba864469d3eddd3ad511d82a10d2faab5b4bdb3772f4f9a7a0daad6b3414ce3.md)

    This file is an character special file on UNIX/Linux systems. 

* [block_special](group___runtime_file_1ggaabba864469d3eddd3ad511d82a10d2faabd6e8c314153f27213858e6c99602d19.md)

    This file is an block special file on UNIX/Linux systems. 

