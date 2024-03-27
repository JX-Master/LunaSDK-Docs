# Luna::VG::COMMAND_MOVE_TO

```c++
constexpr f32 COMMAND_MOVE_TO = 1.0f
```

The command code that begins one new path. 

This command takes 3 points: {COMMAND_MOVE_TO, X, Y}* X: The x coordinates of the initial position.

* Y: The y coordinates of the initial position.

The former path will be closed when one begin command is detected. 

