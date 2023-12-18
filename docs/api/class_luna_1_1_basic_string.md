# Luna::BasicString
The basic string implementation that is suitable for any character types. 

```c++
class Luna::BasicString
```

## Static objects
* [constexpr usize npos](class_luna_1_1_basic_string_1aba46fb9e7bfa2d6d109cc138bfa6cc11.md)

    A special value that usually represents the end of the string. The exact meaning of this value is content specific. 

## Member functions
* [BasicString()](class_luna_1_1_basic_string_1a99b7e53beaad2f733610d81ef6a9b1b3.md)

    Constructs one empty string. 

* [BasicString(const allocator_type &alloc)](class_luna_1_1_basic_string_1a6c0a82f3de42674e9dcb2b0feb197c89.md)

    Constructs one empty string with an custom allocator. 

* [BasicString(usize count, value_type ch, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1a1ee0650700e2381cf3bb559f79d3977c.md)

    Constructs one string using `count` copies of character `ch`. 

* [BasicString(const BasicString &rhs, usize pos, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1ab1ddce60a63968c3164db74b7985a633.md)

    Constructs one string by coping characters in range from another string. 

* [BasicString(const BasicString &rhs, usize pos, usize count, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1a395f88c6f8d82c1457016cc8631d8cd9.md)

    Constructs one string by coping characters from another string. 

* [BasicString(const value_type *s, usize count, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1a8b30bdadfac9679bf69af0038aa2b349.md)

    Constructs one string by coping characters from the provided character array. 

* [BasicString(const value_type *s, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1aa1eb74d3f10f90bbc051379d4c24c877.md)

    Constructs one string by coping characters from the provided null-terminated C string. The length of the string is determined by the first null character. 

* [BasicString(_InputIt first, _InputIt last, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1ae51d3dcd5d954aec9dfe0d29158f28fc.md)

    Constructs one string by coping characters from string specified by the iterator range. 

* [BasicString(const BasicString &rhs)](class_luna_1_1_basic_string_1a83f63a3df66cad6864a93bf7d084d86f.md)

    Constructs one string by coping data from another string. 

* [BasicString(const BasicString &rhs, const allocator_type &alloc)](class_luna_1_1_basic_string_1abe9148da7cef9295ac0f3a19f3827a8f.md)

    Constructs one string by coping data from another string. 

* [BasicString(BasicString &&rhs)](class_luna_1_1_basic_string_1a4a5e43dfb28d6d896330d93e08e586f1.md)

    Constructs one string by moving data from another string. 

* [BasicString(BasicString &&rhs, const allocator_type &alloc)](class_luna_1_1_basic_string_1a3a7dae1bd385fed0001bbb2050e43420.md)

    Constructs one string by moving data from another string. 

* [BasicString(InitializerList< value_type > ilist, const allocator_type &alloc=allocator_type())](class_luna_1_1_basic_string_1aa2ce505de2f748a6e19d1794994c37ab.md)

    Constructs one string by coping characters from the initializer list. 

* [BasicString< _Char, _Alloc > & operator=(const BasicString &rhs)](class_luna_1_1_basic_string_1aaa68857828bafc0623a557fef4cc08d0.md)

    Assigns the string by coping data from another string. 

* [BasicString< _Char, _Alloc > & operator=(BasicString &&rhs)](class_luna_1_1_basic_string_1afd21ac16c47a32a9d74913813889ddee.md)

    Assigns the string by moving data from another string. 

* [BasicString< _Char, _Alloc > & operator=(const value_type *s)](class_luna_1_1_basic_string_1afccbb78b6d303ec2d0d52625b6d08c50.md)

    Assigns the string by coping characters from the provided null-terminated C string. The length of the string is determined by the first null character. 

* [BasicString< _Char, _Alloc > & operator=(value_type ch)](class_luna_1_1_basic_string_1a32ddf9322e658dae867e4a2087730437.md)

    Assigns the string with the specified character. This operation behaves the same as `assign(1, ch)`. 

* [BasicString< _Char, _Alloc > & operator=(InitializerList< value_type > ilist)](class_luna_1_1_basic_string_1ab68db2182b22db4644c7a35e111735c5.md)

    Assigns the string by coping characters from the initializer list. 

* [BasicString< _Char, _Alloc >::pointer data()](class_luna_1_1_basic_string_1abbe2708e47e4589174382b703afa3f15.md)

    Gets one pointer to the underlying character data. 

* [BasicString< _Char, _Alloc >::const_pointer data() const](class_luna_1_1_basic_string_1a567c2df51a74b4f19d20d96a35ffeca4.md)

    Gets one constant pointer to the underlying character data. 

* [BasicString< _Char, _Alloc >::const_pointer c_str() const](class_luna_1_1_basic_string_1ab63a641601252a6a8ddd2b28ee6d19b7.md)

    Gets a non-modifiable C string pointer to the characters stored by this string. 

* [BasicString< _Char, _Alloc >::iterator begin()](class_luna_1_1_basic_string_1a485fe7e9c808bf76d4d707dd41bb660c.md)

    Gets one iterator to the first character of this string. 

* [BasicString< _Char, _Alloc >::iterator end()](class_luna_1_1_basic_string_1ac1e1899a911bdc63af843a842ab0e1ce.md)

    Gets one iterator to the one-past-last character of this string. 

* [BasicString< _Char, _Alloc >::const_iterator begin() const](class_luna_1_1_basic_string_1a0743aee1de77906b3821efe2ceb6a993.md)

    Gets one constnat iterator to the first character of this string. 

* [BasicString< _Char, _Alloc >::const_iterator end() const](class_luna_1_1_basic_string_1aab3443be8bc262a0605a51404e009a41.md)

    Gets one constant iterator to the one-past-last character of this string. 

* [BasicString< _Char, _Alloc >::const_iterator cbegin() const](class_luna_1_1_basic_string_1a12ddc1282e2a1aa2ae3c223f17242b65.md)

    Gets one constnat iterator to the first character of this string. 

* [BasicString< _Char, _Alloc >::const_iterator cend() const](class_luna_1_1_basic_string_1a0fe017ccad383b030905b0585a189ba2.md)

    Gets one constant iterator to the one-past-last character of this string. 

* [BasicString< _Char, _Alloc >::reverse_iterator rbegin()](class_luna_1_1_basic_string_1a9e4772510e9a5d712a7584d749607fdd.md)

    Gets one reverse iterator to the last character of this string. 

* [BasicString< _Char, _Alloc >::reverse_iterator rend()](class_luna_1_1_basic_string_1a25e5bdb3b6da21716b331c2be9b4b291.md)

    Gets one reverse iterator to the one-before-first character of this string. 

* [BasicString< _Char, _Alloc >::const_reverse_iterator rbegin() const](class_luna_1_1_basic_string_1abed8b64cd6c1602b7ac61866643b6ebb.md)

    Gets one constant reverse iterator to the last character of this string. 

* [BasicString< _Char, _Alloc >::const_reverse_iterator rend() const](class_luna_1_1_basic_string_1ae0d186070a94a1440ffe9d6cef20ea6a.md)

    Gets one constant reverse iterator to the one-before-first character of this string. 

* [BasicString< _Char, _Alloc >::const_reverse_iterator crbegin() const](class_luna_1_1_basic_string_1a7f221d4c41cbdb0441a68c27f784db02.md)

    Gets one constant reverse iterator to the last character of this string. 

* [BasicString< _Char, _Alloc >::const_reverse_iterator crend() const](class_luna_1_1_basic_string_1a664b99ac36d39def6786e3910f1c584f.md)

    Gets one constant reverse iterator to the one-before-first character of this string. 

* [usize size() const](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the string, that is, the number of characters in the string, excluding the null terminator. 

* [usize length() const](class_luna_1_1_basic_string_1a0070827b4bc9e3599ef863b636429405.md)

    Gets the size of the string, that is, the number of characters in the string, excluding the null terminator. 

* [usize capacity() const](class_luna_1_1_basic_string_1ad96bf59cb22e917cbd210ba068e8acb3.md)

    Gets the capacity of the string, that is, the maximum number of characters that can be stored in this string without reallocating the string buffer. 

* [bool empty() const](class_luna_1_1_basic_string_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this string is empty, that is, the size of this string is `0`. 

* [void reserve(usize new_cap)](class_luna_1_1_basic_string_1aa1c32ac6498d3f6d21cab98d1cbf3455.md)

    Increases the capacity of the string to a value greater than or equal to `new_cap`, so that it can hold at least `new_cap` characters without reallocating the string buffer. 

* [void resize(usize n, value_type v)](class_luna_1_1_basic_string_1a5f593a1528c4bf10a399df35cf672471.md)

    Resizes the string. 

* [void shrink_to_fit()](class_luna_1_1_basic_string_1a5f16304f80b6fb253c7b0ead3e16dd18.md)

    Reduces the capacity of the string so that [capacity](class_luna_1_1_basic_string_1ad96bf59cb22e917cbd210ba068e8acb3.md) == [size](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md). 

* [BasicString< _Char, _Alloc >::reference operator[](usize n)](class_luna_1_1_basic_string_1aff53b570b2210308aaa7f06812a3aae5.md)

    Gets the character at the specified index. 

* [BasicString< _Char, _Alloc >::const_reference operator[](usize n) const](class_luna_1_1_basic_string_1ae934b86c6f615491ff2980defa42bda8.md)

    Gets the character at the specified index. 

* [BasicString< _Char, _Alloc >::reference at(usize n)](class_luna_1_1_basic_string_1a39e8fb7c2927d86ef30febefef007df3.md)

    Gets the character at the specified index. 

* [BasicString< _Char, _Alloc >::const_reference at(usize n) const](class_luna_1_1_basic_string_1a594c723cd2712f9d9de563449f67314b.md)

    Gets the character at the specified index. 

* [BasicString< _Char, _Alloc >::reference front()](class_luna_1_1_basic_string_1a390f65a29dcf8221ec59217d048e2da6.md)

    Gets the first character of the string. 

* [BasicString< _Char, _Alloc >::const_reference front() const](class_luna_1_1_basic_string_1ac82fd6c57c265dda778ba0f891d950b6.md)

    Gets the first character of the string. 

* [BasicString< _Char, _Alloc >::reference back()](class_luna_1_1_basic_string_1ab2ef2e01ee52e9e351b8c7d37eee9ace.md)

    Gets the last character of the string. 

* [BasicString< _Char, _Alloc >::const_reference back() const](class_luna_1_1_basic_string_1a327634daff2da0da7f0e64f1e6ec466a.md)

    Gets the last character of the string. 

* [void clear()](class_luna_1_1_basic_string_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all characters from the string, but keeps the string buffer. 

* [void push_back(value_type ch)](class_luna_1_1_basic_string_1abdeab95d5acfa0439baf748a61bd3e44.md)

    Pushes one character to the back of the string. 

* [void pop_back()](class_luna_1_1_basic_string_1a058bda4957df6a97b1ea6c9fd783f672.md)

    Removes the element from the back of the string. 

* [void assign(usize count, value_type ch)](class_luna_1_1_basic_string_1acaca48746d4231a8a7efa00bcb7b3f38.md)

    Assigns the string data by `count` copies of `ch`. 

* [void assign(const BasicString &str)](class_luna_1_1_basic_string_1a08afab21726dbca77163d7bd1048bd35.md)

    Assigns the string data by coping characters from another string. 

* [void assign(const BasicString &str, usize pos, usize count=npos)](class_luna_1_1_basic_string_1a4193eddfc9b5ff95df7be38e96c28cdd.md)

    Assigns the string data by coping characters from one subrange of another string. 

* [void assign(BasicString &&str)](class_luna_1_1_basic_string_1ad9aaac0c8ce1d96919f7cbbdb8c08e25.md)

    Assigns the string data by moving characters from another string. 

* [void assign(const value_type *s, usize count)](class_luna_1_1_basic_string_1abae828c38f73a823032b1c79359a20f1.md)

    Assigns the string data by coping characters from the provided character array. 

* [void assign(const value_type *s)](class_luna_1_1_basic_string_1aacb033acdc0e46a3f6d008ca05769e7e.md)

    Assigns the string data by coping characters from the provided null-terminated C string. The length of the string is determined by the first null character. 

* [void assign(_InputIt first, _InputIt last)](class_luna_1_1_basic_string_1aee2d3f122495a2e6b4a96d5873e41404.md)

    Assigns the string data by coping characters from string specified by the iterator range. 

* [void assign(InitializerList< value_type > ilist)](class_luna_1_1_basic_string_1af80ee60b2d616a86fe008cf226795f26.md)

    Assigns the string data by coping characters from the initializer list. 

* [void insert(usize index, usize count, value_type ch)](class_luna_1_1_basic_string_1a1e444be7fe7ef066046732cb9310f1c8.md)

    Inserts `count` copies of characters in the specified position. 

* [void insert(usize index, const value_type *s)](class_luna_1_1_basic_string_1a5b1ac80d4ddf86a18a60c93cbf9e1194.md)

    Inserts one null-terminated C string at the specified position. 

* [void insert(usize index, const value_type *s, usize count)](class_luna_1_1_basic_string_1ad584a2af756ad452e13eaccc4f2462b8.md)

    Inserts one character array at the specified position. 

* [void insert(usize index, const BasicString &str)](class_luna_1_1_basic_string_1ad33a77a2cb62c03539130888b144edad.md)

    Inserts another string at the specified position. 

* [void insert(usize index, const BasicString &str, usize index_str, usize count)](class_luna_1_1_basic_string_1a496120a9d0bb9092d8f9871e25452b7a.md)

    Inserts one subrange of another string at the specified position. 

* [BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, value_type ch)](class_luna_1_1_basic_string_1a9d7c20377f364e713b8f4a6af0c80554.md)

    Inserts one character at the specified position. 

* [BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, usize count, value_type ch)](class_luna_1_1_basic_string_1a086ca2e7c9a1d4e090567cc7409ae23d.md)

    Inserts `count` copies of `ch` at the specified position. 

