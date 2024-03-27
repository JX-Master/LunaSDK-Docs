# Luna::RHI::RasterizerDesc::depth_clip_enable

```c++
bool depth_clip_enable
```

Whether to discard fragments outside of the allowed depth range (0~1). If this is `false`, outside fragments will have their depth values clamped to [`0`, `1`]. 

