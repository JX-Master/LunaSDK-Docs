# Luna::inverse

```c++
Float4x4 inverse(const Float4x4 &mat, f32 *out_determinant=nullptr)
```

Computes the inversed matrix of the specified matrix. 

This function performs the following operations: 
```
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) det = [determinant](group___runtime_math_1gac65d53221bef8dc9fba445639223af92.md)(m);
if (out_determinant)
{
    *out_determinant = det;
}
if (det > -F32_EPSILON && det < F32_EPSILON)
{
    det = F32_EPSILON;
}
[f32](group___runtime_base_type_1gad34d88453d37b65a09797bad37f2f527.md) det_inv = 1.0f / det;
Float4x4 [r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md);
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[0].x =  det_inv * (mat.r[1].y * (mat.r[2].z * mat.r[3].w - mat.r[2].w * mat.r[3].z) + mat.r[1].z * (mat.r[2].w * mat.r[3].y - mat.r[2].y * mat.r[3].w) + mat.r[1].w * (mat.r[2].y * mat.r[3].z - mat.r[2].z * mat.r[3].y));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[1].x = -det_inv * (mat.r[1].x * (mat.r[2].z * mat.r[3].w - mat.r[2].w * mat.r[3].z) + mat.r[1].z * (mat.r[2].w * mat.r[3].x - mat.r[2].x * mat.r[3].w) + mat.r[1].w * (mat.r[2].x * mat.r[3].z - mat.r[2].z * mat.r[3].x));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[2].x =  det_inv * (mat.r[1].x * (mat.r[2].y * mat.r[3].w - mat.r[2].w * mat.r[3].y) + mat.r[1].y * (mat.r[2].w * mat.r[3].x - mat.r[2].x * mat.r[3].w) + mat.r[1].w * (mat.r[2].x * mat.r[3].y - mat.r[2].y * mat.r[3].x));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[3].x = -det_inv * (mat.r[1].x * (mat.r[2].y * mat.r[3].z - mat.r[2].z * mat.r[3].y) + mat.r[1].y * (mat.r[2].z * mat.r[3].x - mat.r[2].x * mat.r[3].z) + mat.r[1].z * (mat.r[2].x * mat.r[3].y - mat.r[2].y * mat.r[3].x));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[0].y = -det_inv * (mat.r[0].y * (mat.r[2].z * mat.r[3].w - mat.r[2].w * mat.r[3].z) + mat.r[0].z * (mat.r[2].w * mat.r[3].y - mat.r[2].y * mat.r[3].w) + mat.r[0].w * (mat.r[2].y * mat.r[3].z - mat.r[2].z * mat.r[3].y));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[1].y =  det_inv * (mat.r[0].x * (mat.r[2].z * mat.r[3].w - mat.r[2].w * mat.r[3].z) + mat.r[0].z * (mat.r[2].w * mat.r[3].x - mat.r[2].x * mat.r[3].w) + mat.r[0].w * (mat.r[2].x * mat.r[3].z - mat.r[2].z * mat.r[3].x));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[2].y = -det_inv * (mat.r[0].x * (mat.r[2].y * mat.r[3].w - mat.r[2].w * mat.r[3].y) + mat.r[0].y * (mat.r[2].w * mat.r[3].x - mat.r[2].x * mat.r[3].w) + mat.r[0].w * (mat.r[2].x * mat.r[3].y - mat.r[2].y * mat.r[3].x));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[3].y =  det_inv * (mat.r[0].x * (mat.r[2].y * mat.r[3].z - mat.r[2].z * mat.r[3].y) + mat.r[0].y * (mat.r[2].z * mat.r[3].x - mat.r[2].x * mat.r[3].z) + mat.r[0].z * (mat.r[2].x * mat.r[3].y - mat.r[2].y * mat.r[3].x));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[0].z =  det_inv * (mat.r[3].w * (mat.r[0].y * mat.r[1].z - mat.r[0].z * mat.r[1].y) + mat.r[3].z * (mat.r[0].w * mat.r[1].y - mat.r[0].y * mat.r[1].w) + mat.r[3].y * (mat.r[0].z * mat.r[1].w - mat.r[0].w * mat.r[1].z));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[1].z = -det_inv * (mat.r[3].w * (mat.r[0].x * mat.r[1].z - mat.r[0].z * mat.r[1].x) + mat.r[3].z * (mat.r[0].w * mat.r[1].x - mat.r[0].x * mat.r[1].w) + mat.r[3].x * (mat.r[0].z * mat.r[1].w - mat.r[0].w * mat.r[1].z));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[2].z =  det_inv * (mat.r[3].w * (mat.r[0].x * mat.r[1].y - mat.r[0].y * mat.r[1].x) + mat.r[3].y * (mat.r[0].w * mat.r[1].x - mat.r[0].x * mat.r[1].w) + mat.r[3].x * (mat.r[0].y * mat.r[1].w - mat.r[0].w * mat.r[1].y));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[3].z = -det_inv * (mat.r[3].z * (mat.r[0].x * mat.r[1].y - mat.r[0].y * mat.r[1].x) + mat.r[3].y * (mat.r[0].z * mat.r[1].x - mat.r[0].x * mat.r[1].z) + mat.r[3].x * (mat.r[0].y * mat.r[1].z - mat.r[0].z * mat.r[1].y));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[0].w = -det_inv * (mat.r[2].w * (mat.r[0].y * mat.r[1].z - mat.r[0].z * mat.r[1].y) + mat.r[2].z * (mat.r[0].w * mat.r[1].y - mat.r[0].y * mat.r[1].w) + mat.r[2].y * (mat.r[0].z * mat.r[1].w - mat.r[0].w * mat.r[1].z));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[1].w =  det_inv * (mat.r[2].w * (mat.r[0].x * mat.r[1].z - mat.r[0].z * mat.r[1].x) + mat.r[2].z * (mat.r[0].w * mat.r[1].x - mat.r[0].x * mat.r[1].w) + mat.r[2].x * (mat.r[0].z * mat.r[1].w - mat.r[0].w * mat.r[1].z));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[2].w = -det_inv * (mat.r[2].w * (mat.r[0].x * mat.r[1].y - mat.r[0].y * mat.r[1].x) + mat.r[2].y * (mat.r[0].w * mat.r[1].x - mat.r[0].x * mat.r[1].w) + mat.r[2].x * (mat.r[0].y * mat.r[1].w - mat.r[0].w * mat.r[1].y));
[r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md).r[3].w =  det_inv * (mat.r[2].z * (mat.r[0].x * mat.r[1].y - mat.r[0].y * mat.r[1].x) + mat.r[2].y * (mat.r[0].z * mat.r[1].x - mat.r[0].x * mat.r[1].z) + mat.r[2].x * (mat.r[0].y * mat.r[1].z - mat.r[0].z * mat.r[1].y));
return [r](group___h_i_d_1gga912f74cfa86bfd7af0ee6bb9010eba51a4b43b0aee35624cd95b910189b3dc231.md);
```


## Parameters
* *in* **mat**

    The matrix to compute. 

* *out* **out_determinant**

    If not `nullptr`, returns the determinant of `mat`. 

## Return value
Returns the inversed matrix of the specified matrix. 

