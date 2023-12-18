# Luna::Array
Represents one array of fixed or dynamic size. 

```c++
class Luna::Array
```

[Array](class_luna_1_1_array.md) is one container that contains fixed number of elements. The size of one array can be set in compile time by specifying `_Size` of the array, or can be set when creating the array by setting `_Size` to [DYNAMIC_ARRAY_SIZE](group___runtime_container_1gac211fb2fcac88253a56c67d77c041a02.md). Unlike [Vector](class_luna_1_1_vector.md), the size of one array cannot be changed after the array is created. If the size of the array is determined in compile time, the memory for elements will be allocated directly in the array object; if the size of the array is determined in run time, the memory for elements will be allocated dynamically on heap. 

## Member functions
* [constexpr reference at(usize pos)](class_luna_1_1_array_1a4246559492a9ac95f5fd5e33e5077cc0.md)

    Gets a refernece of the element at the specified index. 

* [constexpr const_reference at(usize pos) const](class_luna_1_1_array_1a48ec46b8d8158353cf7a248921ea86ab.md)

    Gets a const refernece of the element at the specified index. 

* [constexpr reference operator[](usize pos)](class_luna_1_1_array_1a534b7f2bfb1e389b9e6b6fcb8370f1db.md)

    Gets a refernece of the element at the specified index. 

* [constexpr const_reference operator[](usize pos) const](class_luna_1_1_array_1a79bf825ddf829c374672530695abc932.md)

    Gets a constant refernece of the element at the specified index. 

* [constexpr reference front()](class_luna_1_1_array_1a2fe69b85aade6c6032f22eb79b1b746d.md)

    Gets a reference to the first (index 0) element in the array. 

* [constexpr const_reference front() const](class_luna_1_1_array_1a0d2f4af381faa34ace382c87aeed32e3.md)

    Gets a constant reference to the first (index 0) element in the array. 

* [constexpr reference back()](class_luna_1_1_array_1ae869682a778dc77a8dd62bbfa22f9d9a.md)

    Gets a reference to the last (index `size()` - 1) element in the array. 

* [constexpr const_reference back() const](class_luna_1_1_array_1a20a48cfbeb064093c00708b233c17883.md)

    Gets a reference to the last (index `size()` - 1) element in the array. 

* [constexpr _Ty * data()](class_luna_1_1_array_1aaf0bf16ebc5c8c11cb351557b61e4b9c.md)

    Gets one pointer to the array data memory. 

* [constexpr const _Ty * data() const](class_luna_1_1_array_1a56951c300ecc03279ad99858d6213449.md)

    Gets one constant pointer to the array data memory. 

* [constexpr iterator begin()](class_luna_1_1_array_1a82061640a279283f5d16614b196fcd1d.md)

    Gets one iterator to the first element of the array. 

* [constexpr const_iterator begin() const](class_luna_1_1_array_1a43564d19bdbc133e4a81cc1a2c002254.md)

    Gets one constant iterator to the first element of the array. 

* [constexpr const_iterator cbegin() const](class_luna_1_1_array_1a098840b38d4f639ee9f69cf026be323c.md)

    Gets one constant iterator to the first element of the array. 

* [constexpr iterator end()](class_luna_1_1_array_1afe07af266a2f066a51af64000d746cb9.md)

    Gets one iterator to the one past last element of the array. 

* [constexpr const_iterator end() const](class_luna_1_1_array_1a428cfcc26f33036be7c76ab287ea06c5.md)

    Gets one constant iterator to the one past last element of the array. 

* [constexpr const_iterator cend() const](class_luna_1_1_array_1abee57f5c6cacf03f590795737d18e7e8.md)

    Gets one constant iterator to the one past last element of the array. 

* [constexpr reverse_iterator rbegin()](class_luna_1_1_array_1a3c6e58d7002c8e81a78dcd3b59a4e396.md)

    Gets one reverse iterator to the last element of the array. 

* [constexpr const_reverse_iterator rbegin() const](class_luna_1_1_array_1a68e95b44627370eea593b039c42e1244.md)

    Gets one constant reverse iterator to the last element of the array. 

* [constexpr const_reverse_iterator crbegin() const](class_luna_1_1_array_1a0c080710404cf54608566718e135ed4e.md)

    Gets one constant reverse iterator to the last element of the array. 

* [constexpr reverse_iterator rend()](class_luna_1_1_array_1a35220c6806307b7311a170920af27d26.md)

    Gets one reverse iterator to the one-before-first element of the array. 

* [constexpr const_reverse_iterator rend() const](class_luna_1_1_array_1a6e277fde54bd8a8e10e5967deaa68eb1.md)

    Gets one constant reverse iterator to the one-before-first element of the array. 

* [constexpr const_reverse_iterator crend() const](class_luna_1_1_array_1a56d3a1867f42d8f5551c9771bf6ec06f.md)

    Gets one constant reverse iterator to the one-before-first element of the array. 

* [constexpr bool empty() const](class_luna_1_1_array_1afaafdfc441c2433c70959e3dfe46fd97.md)

    Checks whether this array is empty, that is, the size of this array is `0`. 

* [constexpr usize size() const](class_luna_1_1_array_1adb59c183f075f048ae90778d15189686.md)

    Gets the size of the array. 

* [constexpr void fill(const _Ty &value)](class_luna_1_1_array_1a39c2d1119b91eb075fc6d9a5910dbebd.md)

    Assigns every element in the array with the specified value. 

* [constexpr void swap(Array &rhs)](class_luna_1_1_array_1a2f476cf713d1e863951ed725acf89284.md)

    Swaps content of this array with another array of the same element type and size. 

