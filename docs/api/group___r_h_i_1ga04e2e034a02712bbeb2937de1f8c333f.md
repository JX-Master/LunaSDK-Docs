# Luna::RHI::PrimitiveTopology

```c++
enum PrimitiveTopology : u8
{
    point_list
    line_list
    line_strip
    triangle_list
    triangle_strip
}
```

Specifies the primitive type for the graphics pipeline to draw. 

## Options
* [point_list](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333faca5a3df0ee5e40625a9623f463ac519e.md)

    Draws point list, where every vertex in the vertex buffer specifies one point. 

* [line_list](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333fa09adbdc7b6551c6c4e2ab8ebbfdb23fb.md)

    Draws line list, where every two continious vertices in the vertex buffer specify two points of one line. 

* [line_strip](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333fa7441cbdc45313ce65d3606b1d6e403dd.md)

    Draws line strip, where every vertex and its prior vertex in the vertex buffer specify two points of one line. 

* [triangle_list](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333fae7d7946aa0047daaed3121d34463184f.md)

    Draws triangle list, where every three continious vertices in the vertex buffer specify three points of one triangle. 

* [triangle_strip](group___r_h_i_1gga04e2e034a02712bbeb2937de1f8c333fa01edf5f1ae6135daec55d230c83d3885.md)

    Draws line strip, where every vertex and its prior two vertices in the vertex buffer specify three points of one triangle. 

