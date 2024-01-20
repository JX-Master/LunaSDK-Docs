# Transform operations
## Functions
* [Float3x3 make(const Float2 &translation, f32 rotation, const Float2 &scaling)](group___runtime_math_transform_1ga2bb0c38d21068c718d00d96fe8276617.md)

    Constructs one 2D affine matrix. 

* [Float4x4 make(const Float3 &translation, const Float4 &rotation, const Float3 &scaling)](group___runtime_math_transform_1ga6b9687ba718a4cd807b3d01d6956b900.md)

    Constructs one 3D affine matrix. 

* [Float2 up(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga2f76168e375689235f22dd1c2505d67a.md)

    Extracts the up direction from one 2D affine matrix. 

* [Float3 up(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga15e995b58587b0510d95aa5b0e48ad17.md)

    Extracts the up direction from one 3D affine matrix. 

* [Float2 down(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga2a69d5278be67ec9142d8203c093fd92.md)

    Extracts the down direction from one 2D affine matrix. 

* [Float3 down(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga19911158ef0a2f09640b26d92a6e082e.md)

    Extracts the down direction from one 3D affine matrix. 

* [Float2 left(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga1cac457659fb08caf3b454f3f7fb4896.md)

    Extracts the left direction from one 2D affine matrix. 

* [Float3 left(const Float4x4 &affine_matrix)](group___runtime_math_transform_1gae5cb346d045ce2f830ce26ab46642a85.md)

    Extracts the left direction from one 3D affine matrix. 

* [Float2 right(const Float3x3 &affine_matrix)](group___runtime_math_transform_1gad9cdacb22d22a524dc94551b3a60e8a0.md)

    Extracts the right direction from one 2D affine matrix. 

* [Float3 right(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga480d65cf4c507e988a3d4bb742b994c2.md)

    Extracts the right direction. 

* [Float3 forward(const Float4x4 &affine_matrix)](group___runtime_math_transform_1gafd6130d43d23bb950a06ecd38d434964.md)

    Extracts the forward direction from one 3D affine matrix. 

* [Float3 backward(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga5d7832146bee663814bb11e99172e1e3.md)

    Extracts the backward direction from one 3D affine matrix. 

* [Float2 translation(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga6dc9a198d3e71feddc15327360fecbfb.md)

    Extracts the translation component from one 2D affine matrix. 

* [Float3 translation(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga84607afb65ff2b3286b7b5bc5e9756f9.md)

    Extracts the translation component from one 3D affine matrix. 

* [f32 rotation(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga633216e90f210b64adfd5546b97f4a3b.md)

    Extracts the rotation component from one 2D affine matrix. 

* [Float4 rotation(const Float4x4 &rotation_matrix)](group___runtime_math_transform_1ga1eb43c4d3f90fa4c83daf53826cb16dc.md)

    Computes the quaternion from one rotation matrix. 

* [Float3 euler_angles(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga0162e4e733860f68ae63653815b2365d.md)

    Computes the euler angles from one rotation matrix. 

* [Float2 scaling(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga10ba4b2f0018784e41f9dd39c32f2d7d.md)

    Extracts the scaling component from one 2D affine matrix. 

* [Float3 scaling(const Float4x4 &affine_matrix)](group___runtime_math_transform_1gac89f80fd9a3385161791be05a30d774a.md)

    Extracts the scaling component from one 3D affine matrix. 

* [Float3x3 translation_matrix(const Float3x3 &affine_matrix)](group___runtime_math_transform_1gae0a729ca62103b1a737d366d0c367ad3.md)

    Extracts the translation matrix from one 2D affine matrix. 

* [Float4x4 translation_matrix(const Float4x4 &affine_matrix)](group___runtime_math_transform_1gad4a791677330d07a983e15f0d10be380.md)

    Extracts the translation matrix from one 3D affine matrix. 

* [Float3x3 rotation_matrix(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga032e2fe95d08cca4b502e7e9f709061a.md)

    Extracts the rotation matrix from one 2D affine matrix. 

* [Float4x4 rotation_matrix(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga7c8fb28fc3c336b112ba54cb25d5a9f0.md)

    Extracts the rotation matrix from one 3D affine matrix. 

* [Float3x3 scaling_matrix(const Float3x3 &affine_matrix)](group___runtime_math_transform_1ga51241e57c06a265e83502141b01a78cc.md)

    Extracts the scaling matrix from one 2D affine matrix. 

* [Float4x4 scaling_matrix(const Float4x4 &affine_matrix)](group___runtime_math_transform_1ga143f9c09fbd615dcf7142e1ae47d1c50.md)

    Extracts the scaling matrix from one 3D affine matrix. 

* [Float3x3 make_translation(const Float2 &translation)](group___runtime_math_transform_1gaaa7e76d9b8452dd685ed91941a4da7fb.md)

    Constructs one 2D translation matrix from one translation vector. 

* [Float3x3 make_translation(f32 x, f32 y)](group___runtime_math_transform_1ga96faa304571fbd589feeef42ab0c87c8.md)

    Constructs one 2D translation matrix from x and y position. 

* [Float4x4 make_translation(const Float3 &translation)](group___runtime_math_transform_1ga8b1eb3ec30835524690271fd4447590a.md)

    Constructs one 3D translation matrix from one translation vector. 

* [Float4x4 make_translation(f32 x, f32 y, f32 z)](group___runtime_math_transform_1ga4e778805ef74fb61ff3456357d89facc.md)

    Constructs one 3D translation matrix from x, y and z position. 

* [Float3x3 make_rotation(f32 rotation)](group___runtime_math_transform_1gaff7a0374cf30a756043abfa616f93a96.md)

    Constructs one 2D rotation matrix from one rotation scalar. 

* [Float4x4 make_rotation(const Float4 &rotation)](group___runtime_math_transform_1ga9aaba0783915d41bd3ce16bb0cd3b311.md)

    Constructs one 3D rotation matrix from one rotation Quaternion. 

* [Float4x4 make_rotation_x(f32 angle)](group___runtime_math_transform_1ga1b64a4f154172730a7bf60ebedd15820.md)

    Constructs one 3D rotation matrix that represents one rotation alone x axis. 

* [Float4x4 make_rotation_y(f32 angle)](group___runtime_math_transform_1gade3bece16fa5ae3ac350d981b3ded2bf.md)

    Constructs one 3D rotation matrix that represents one rotation alone y axis. 

* [Float4x4 make_rotation_z(f32 angle)](group___runtime_math_transform_1ga5737ff212e0048cad34ab98bde89de3e.md)

    Constructs one 3D rotation matrix that represents one rotation alone z axis. 

* [Float4x4 make_rotation_axis_angle(const Float3 &axis, f32 angle)](group___runtime_math_transform_1ga49761a03e8b53306eec4f57c899cd3e6.md)

    Constructs one 3D rotation matrix by specifying the rotation axis and rotation angle. 

* [Float4x4 make_rotation_euler_angles(const Float3 &euler_angles)](group___runtime_math_transform_1ga5b7cc1566b23738e6479a8777d909b6c.md)

    Constructs one 3D rotation matrix from Euler angles (pitch, yaw, roll). 

* [Float4x4 make_rotation_euler_angles(f32 pitch, f32 yaw, f32 roll)](group___runtime_math_transform_1gaced26092c32f03251baac8d8fd45bf18.md)

    Constructs one 3D rotation matrix from Euler angles (pitch, yaw, roll). 

* [Float3x3 make_scaling(const Float2 &scaling)](group___runtime_math_transform_1gafd3cb55201dc4fc08d37fc9dd626d51a.md)

    Constructs one 2D scaling matrix from one scaling vector. 

* [Float3x3 make_scaling(f32 scale_x, f32 scale_y)](group___runtime_math_transform_1ga589cb5f29f0fc3ee1d482e4bf8d5b3d4.md)

    Constructs one 2D scaling matrix from scaling factors in x and y directions. 

* [Float4x4 make_scaling(const Float3 &scaling)](group___runtime_math_transform_1ga6ccd284db40cdc964c71c9408b9ef181.md)

    Constructs one 3D scaling matrix from one scaling vector. 

* [Float4x4 make_scaling(f32 scale_x, f32 scale_y, f32 scale_z)](group___runtime_math_transform_1ga3e3dd4cebd1e252aaa701ca3ceef1500.md)

    Constructs one 3D scaling matrix from scaling factors in x, y and z directions. 

* [Float4x4 make_look_at(const Float3 &eye_pos, const Float3 &target_pos, const Float3 &up_dir)](group___runtime_math_transform_1ga4d3ab69162d42a12d77d6b7a767c6807.md)

    Constructs one view matrix that targets the specified position. 

* [Float4x4 make_look_to(const Float3 &eye_pos, const Float3 &eye_dir, const Float3 &up_dir)](group___runtime_math_transform_1ga7c901e41da12595b1779320556c1416b.md)

    Constructs one view matrix that targets the specified direction. 

* [Float4x4 make_perspective(f32 near_width, f32 near_height, f32 near_z, f32 far_z)](group___runtime_math_transform_1gab5b86389fb30a19bee76c16107625937.md)

    Constructs one perspective projection matrix using width, height, near clipping distance and far clipping distance. 

* [Float4x4 make_perspective_fov(f32 fov, f32 aspect_ratio, f32 near_z, f32 far_z)](group___runtime_math_transform_1ga6b90fe4b9e14dd61e00600d525ccbcf6.md)

    Constructs one perspective projection matrix using diagonal fov, aspect_ratio, near clipping distance and far clipping distance. 

* [Float4x4 make_perspective_fov_w(f32 fov_w, f32 aspect_ratio, f32 near_z, f32 far_z)](group___runtime_math_transform_1ga8e558b40b6111633ff80ac3083653a7b.md)

    Constructs one perspective projection matrix using width fov, aspect_ratio, near clipping distance and far clipping distance. 

* [Float4x4 make_perspective_fov_h(f32 fov_h, f32 aspect_ratio, f32 near_z, f32 far_z)](group___runtime_math_transform_1ga36036491d4d444f5d96a9e27027b24b3.md)

    Constructs one perspective projection matrix using height fov, aspect_ratio, near clipping distance and far clipping distance. 

* [Float4x4 make_perspective_off_center(f32 near_left, f32 near_right, f32 near_bottom, f32 near_top, f32 near_z, f32 far_z)](group___runtime_math_transform_1gafa595ebbd744e2c0c546783ff4df26c9.md)

    Constructs one perspective projection matrix using four offset values from the camera center, near clipping distance and far clipping distance. 

* [Float4x4 make_orthographic(f32 width, f32 height, f32 near_z, f32 far_z)](group___runtime_math_transform_1ga2ec91a351a0b0dcbf6f461d09d8603dc.md)

    Constructs one orthographic projection matrix using width, height near clipping distance, and far clipping distance. 

* [Float4x4 make_orthographic_off_center(f32 left, f32 right, f32 bottom, f32 top, f32 near_z, f32 far_z)](group___runtime_math_transform_1gafcbd14a91c56b4a36bc11aa51013988c.md)

    Constructs one orthographic projection matrix using four offset values from the camera center, near clipping distance and far clipping distance. 

