# Luna::SeekMode

```c++
enum SeekMode : u32
{
    begin= 1
    current= 2
    end= 3
}
```

Specify the seek mode for one seekable stream. 

## Options
* [begin](group___runtime_1ggaf2c27cfc991f5e917923e425d0bf1106a8d589afa4dfaeeed85fff5aa78e5ff6a.md)

    The offset is relative to the beginning of the stream. 

* [current](group___runtime_1ggaf2c27cfc991f5e917923e425d0bf1106a43b5c9175984c071f30b873fdce0a000.md)

    The offset is relative to the current position of the cursor. 

* [end](group___runtime_1ggaf2c27cfc991f5e917923e425d0bf1106a7f021a1415b86f2d013b2618fb31ae53.md)

    The offset is relative to the end of the stream. 

