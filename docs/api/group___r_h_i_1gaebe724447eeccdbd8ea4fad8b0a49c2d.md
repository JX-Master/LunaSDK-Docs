# Luna::RHI::MemoryType

```c++
enum MemoryType : u8
{
    local= 0
    upload= 1
    readback= 2
}
```

Specify the memory type. See remarks for details. 



## Remark
The memory type determines the memory location and access policy for the memory. The system will choose the most suitable heap to allocate memory based on the target platform and the specified memory type.


The local memory type is allocated on memory that is visible only to GPU. Such memory gains maximum GPU bandwidth, but cannot be accessed by CPU. On platforms with non-uniform memory architecture (NUMA), the local memory will be allocated on video memory, which cannot be accessed by CPU; in a platform with uniform memory architecture (UMA), the local memory will be allocated on system memory. While it is technically possible for CPU to access local memory on UMA, preventing such access gives the hardware and driver more rooms for optimizing GPU access efficiency.

The upload memory type is allocated on system memory that is optimized for CPU writing. GPU cannot write to this memory and GPU reading from upload memory is slow. On NUMA platfroms, reading data from upload memory from GPU requires data transmission through PCI-Express bus, which is much slower than reading data in local memory from GPU. We recommend using upload memory only for uploading data to local memory or reading the data only once per CPU write.

The readback memory type is allocated on system memory that is optimized for CPU reading. GPU writing to read back memory is slow, and the only operation allowed for GPU is to copy data to the memory. On NUMA platfroms, writing data to readback memory from GPU requires data transmission through PCI-Express bus, which is a slow operation.

The user should choose the suitable memory type based on the use situation. Here are some basic principles:1. If you need to create texture resources, use local memory. If you need to upload texture data from CPU side, use one upload memory to copy data to the local memory.

1. If you don't need to access resource data from CPU, use local memory.

1. If you only need to upload data from CPU side once, like setting the initial data for static vertex and index buffers, use one local memory to store the data, then use one temporary upload memory to copy data to the local memory.

1. If you need to upload data from CPU side multiple times, but the data is read by GPU only once per CPU update, use upload memory.

1. If you need to upload data from CPU side multiple times, and the data will be read by GPU multiple times per CPU update, use one local memory resource for GPU access and one upload memory resource for CPU access, and copy data between two resources when needed.

1. If you need to read resource data from CPU side, use readback memory. 

## Options
* [local](group___r_h_i_1ggaebe724447eeccdbd8ea4fad8b0a49c2daf5ddaf0ca7929578b408c909429f68f2.md)

    The memory can only be read and written by GPU. CPU access is not allowed. 

* [upload](group___r_h_i_1ggaebe724447eeccdbd8ea4fad8b0a49c2da76ee3de97a1b8b903319b7c013d8c877.md)

    The memory can only be written by CPU and read by GPU. Only buffer resources can be created on upload memory. 

* [readback](group___r_h_i_1ggaebe724447eeccdbd8ea4fad8b0a49c2daa29f31235ac8a8050c0221b44da07ebb.md)

    The memory can only be read by CPU and written by GPU. Only buffer resources can be created on readback memory. The buffer resource can only be used as the copy destination for GPU copy commands. 

