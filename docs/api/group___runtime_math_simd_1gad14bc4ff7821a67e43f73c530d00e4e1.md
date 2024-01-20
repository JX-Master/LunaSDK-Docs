# Luna::Simd::modangle_f4

```c++
float4 modangle_f4(float4 a)
```

Computes the per-component angle modulo 2PI for `a`, and stores the results in `dst`. The angle is expressed in radians. The result is rounded in [-PI, PI]. 


```
dst.x := a.x - 2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md) * round( a.x / (2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md)) )
dst.y := a.y - 2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md) * round( a.y / (2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md)) )
dst.z := a.z - 2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md) * round( a.z / (2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md)) )
dst.w := a.w - 2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md) * round( a.w / (2 * [PI](group___runtime_math_1gafce6d114b6c8b3f28b6b051d2c77a760.md)) )
```


