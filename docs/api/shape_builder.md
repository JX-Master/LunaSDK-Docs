# A collection of functions that help generating shape command points.
## Functions
* [void move_to(Vector< f32 > &points, f32 x, f32 y)](group___shape_builder_1gab8e9044200cb869232c488b3e35f6918.md)

    Adds one [COMMAND_MOVE_TO](group___v_g_1ga2bc6953cffc02fae8cda53242fae1faf.md) command to shape data points. 

* [void line_to(Vector< f32 > &points, f32 x, f32 y)](group___shape_builder_1ga013d4c88f23571c1b4bcf5f66c859289.md)

    Adds one [COMMAND_LINE_TO](group___v_g_1ga7517475317efab0dc674d8ac0f0ef425.md) command to shape data points. 

* [void curve_to(Vector< f32 > &points, f32 cx, f32 cy, f32 x, f32 y)](group___shape_builder_1ga4b4fed065aa222c9fa55bc8f0132e8bd.md)

    Adds one [COMMAND_CURVE_TO](group___v_g_1ga24b80fd84c61026f367d5c5d91583621.md) command to shape data points. 

* [void circle_to(Vector< f32 > &points, f32 radius, f32 begin, f32 end)](group___shape_builder_1gab6bd8b68e81680d4e10716393e8960c6.md)

    Adds commands to draw one circle part to shape data points. 

* [void add_rectangle_filled(Vector< f32 > &points, f32 min_x, f32 min_y, f32 max_x, f32 max_y)](group___shape_builder_1ga066d2af97adf8d20d1a30aefeebf3ccc.md)

    Adds commands to draw one filled axis-aligned rectangle. 

* [void add_rectangle_bordered(Vector< f32 > &points, f32 min_x, f32 min_y, f32 max_x, f32 max_y, f32 border_width, f32 border_offset=0.0f)](group___shape_builder_1ga2dda7ca863e8f29cbb2c7579765c19c2.md)

    Adds commands to draw one bordered axis-aligned rectangle. 

* [void add_line(Vector< f32 > &points, f32 p1_x, f32 p1_y, f32 p2_x, f32 p2_y, f32 width, f32 offset=0.0f)](group___shape_builder_1gae11e1fb33e73b1a511c1ad248dc2afeb.md)

    Adds commands to draw one line. 

* [void add_rounded_rectangle_filled(Vector< f32 > &points, f32 min_x, f32 min_y, f32 max_x, f32 max_y, f32 radius)](group___shape_builder_1ga97757e4a868e802d4633b5c0f93d3dab.md)

    Adds commands to draw one filled axis-aligned rounded rectangle. 

* [void add_rounded_rectangle_bordered(Vector< f32 > &points, f32 min_x, f32 min_y, f32 max_x, f32 max_y, f32 radius, f32 border_width, f32 border_offset=0.0f)](group___shape_builder_1ga11055dd3df67653ce45d5071a6886cd3.md)

    Adds commands to draw one bordered axis-aligned rounded rectangle. 

* [void add_circle_filled(Vector< f32 > &points, f32 center_x, f32 center_y, f32 radius)](group___shape_builder_1gaa998cb2d0f146106ef862d37619c8d76.md)

    Adds commands to draw one filled circle. 

* [void add_circle_bordered(Vector< f32 > &points, f32 center_x, f32 center_y, f32 radius, f32 border_width, f32 border_offset=0.0f)](group___shape_builder_1ga8779e46a64cf6b0a3e75568ca409737e.md)

    Adds commands to draw one bordered circle. 

