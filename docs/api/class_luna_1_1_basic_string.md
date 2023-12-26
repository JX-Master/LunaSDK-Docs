# Luna::BasicString
The basic string implementation that is suitable for any character types. 

```c++
template <typename _Char, typename _Alloc>
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

* [void insert(usize index, const BasicString &str, usize index_str, usize count=npos)](class_luna_1_1_basic_string_1a22ef9a75352db0c2f37f3cc5581d0470.md)

    Inserts one subrange of another string at the specified position. 

* [BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, value_type ch)](class_luna_1_1_basic_string_1a9d7c20377f364e713b8f4a6af0c80554.md)

    Inserts one character at the specified position. 

* [BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, usize count, value_type ch)](class_luna_1_1_basic_string_1a086ca2e7c9a1d4e090567cc7409ae23d.md)

    Inserts `count` copies of `ch` at the specified position. 

* [BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, _InputIt first, _InputIt last)](class_luna_1_1_basic_string_1a819ac8c437bf70a69cb028757a2f9cf1.md)

    Inserts characters from the iterator range at the specified position. 

* [BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, InitializerList< value_type > ilist)](class_luna_1_1_basic_string_1af623e3655e9b307d40582f9a274b7d98.md)

    Inserts characters from the specified initializer list at the specified position. 

* [void erase(usize index=0, usize count=npos)](class_luna_1_1_basic_string_1aa545ad0e9ed1fa69cc395a42856cbce4.md)

    Removes `count` characters from the specified position. 

* [BasicString< _Char, _Alloc >::iterator erase(const_iterator pos)](class_luna_1_1_basic_string_1a367811c9cce4501631bd61133b5af24c.md)

    Removes one character. 

* [BasicString< _Char, _Alloc >::iterator erase(const_iterator first, const_iterator last)](class_luna_1_1_basic_string_1a2bd8bd8d9e8f3f1e3d252285f0d0a8f8.md)

    Removes characters in the specified range. 

* [void swap(BasicString &rhs)](class_luna_1_1_basic_string_1a8696fba9dad5e2d99af377769d1ae0c6.md)

    Swaps characters of this string with the specified string. 

* [void append(usize count, value_type ch)](class_luna_1_1_basic_string_1a960d21333a39ee642559f87fd78037a6.md)

    Appends `count` copies of character `ch` to the back of the string. 

* [void append(const BasicString &str)](class_luna_1_1_basic_string_1abad911fa2fe712fc30b6f1371d9ccca1.md)

    Appends another string to the back of the string. 

* [void append(const BasicString &str, usize pos, usize count=npos)](class_luna_1_1_basic_string_1a5524c1733f03a62e069e6269e87fd9d0.md)

    Appends one subrange of another string to the back of the string. 

* [void append(const value_type *s, usize count)](class_luna_1_1_basic_string_1a62dbef30f3cf6cba3cd8e4db913f8ff5.md)

    Appends one character array to the back of the string. 

* [void append(const value_type *s)](class_luna_1_1_basic_string_1abfaf38cfd88e70a7d638d057f3702cb3.md)

    Appends one null-terminated C string to the back of the string. 

* [void append(_InputIt first, _InputIt last)](class_luna_1_1_basic_string_1aa23a815a1690960c24e7531da65f7d74.md)

    Appends characters from the iterator range to the back of the string. 

* [void append(InitializerList< value_type > ilist)](class_luna_1_1_basic_string_1adf931fc77df229e63f55a1cd25fb3105.md)

    Appends characters from the specified initializer list to the back of the string. 

* [i32 compare(const BasicString &rhs) const](class_luna_1_1_basic_string_1a0aa300bc340ead2704f51c0f929041b8.md)

    Compares this string with the specified string. 

* [i32 compare(usize pos1, usize count1, const BasicString &rhs) const](class_luna_1_1_basic_string_1a64605f0e903436fa93460f1e9fbbafad.md)

    Compares [`pos1`, `pos1 + count1`) substring of this string to `rhs`. 

* [i32 compare(usize pos1, usize count1, const BasicString &rhs, usize pos2, usize count2=npos) const](class_luna_1_1_basic_string_1add78057fe7546a3fe35216ccbda5bd50.md)

    Compares a [`pos1`, `pos1 + count1`) substring of this string to a substring [`pos2`, `pos2 + count2`) of `rhs`. 

* [i32 compare(const value_type *s) const](class_luna_1_1_basic_string_1a536e301c18bf7ac0bb43c6b665d06eb2.md)

    Compares this string to the null-terminated C string. 

* [i32 compare(usize pos1, usize count1, const value_type *s) const](class_luna_1_1_basic_string_1afe6fef3ffff75c23d2499957b222173a.md)

    Compares [`pos1`, `pos1 + count1`) substring of this string to the null-terminated C string. 

* [i32 compare(usize pos1, usize count1, const value_type *s, usize count2) const](class_luna_1_1_basic_string_1a47c3a331b179cfd884faef8e88caf293.md)

    Compares [`pos1`, `pos1 + count1`) substring of this string to the characters in the range [`s`, `s + count2`). 

* [void replace(usize pos, usize count, const BasicString &str)](class_luna_1_1_basic_string_1a6d17d834a99bca76c180bd9aee728253.md)

    Replaces characters in range [`pos`, `pos + count`) with characters of `str`. 

* [void replace(const_iterator first, const_iterator last, const BasicString &str)](class_luna_1_1_basic_string_1a6005903a2055c24eaec414fd0f3cdc89.md)

    Replaces characters in range [`first`, `last`) with characters of `str`. 

* [void replace(usize pos, usize count, const BasicString &str, usize pos2, usize count2=npos)](class_luna_1_1_basic_string_1a1e35bd1c2f378b8a51b65c495348aec4.md)

    Replaces characters in range [`pos`, `pos + count`) with a substring [`pos2`, `pos2 + count2`) of `str`. 

* [void replace(const_iterator first, const_iterator last, _InputIt first2, _InputIt last2)](class_luna_1_1_basic_string_1a4b70247166e39d11f67f37b239f326b2.md)

    Replaces characters in range [`first`, `last`) with the characters in the range [`first2`, `last2`). 

* [void replace(usize pos, usize count, const value_type *cstr, usize count2)](class_luna_1_1_basic_string_1a9800e2b9792e254849818ec5861e3a8e.md)

    Replaces characters in range [`pos`, `pos + count`) with a character array [`cstr`, `cstr + count2). @param[in] pos The index of the first character to replace. @param[in] count The number of characters to replace. If`pos + count`is greater than`this->[size()](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md)`,`count`will be clamped to`this->[size()](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md) - pos`. @param[in] cstr The pointer to the character array to use for replacement. @param[in] count2 The number of characters in`cstr`to use for replacement. @par Valid Usage *`pos`must not be greater than`this->[size()](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md)`. 

* [void replace(const_iterator first, const_iterator last, const value_type *cstr, usize count2)](class_luna_1_1_basic_string_1ae6433c006f58290420c9ee6fdd051885.md)

    Replaces characters in range [`first`, `last`) with a character array [`cstr`, `cstr + count2). @param[in] first The iterator to the first character to replace. @param[in] last The iterator to the one-past-last character to replace. @param[in] cstr The pointer to the character array to use for replacement. @param[in] count2 The number of characters in`cstr`to use for replacement. @par Valid Usage. `

* [void replace(usize pos, usize count, const value_type *cstr)](class_luna_1_1_basic_string_1a4b26260265e9a9a22db847a27a3b9941.md)

    Replaces characters in range [`pos`, `pos + count`) with a null-terminated C string. 

* [void replace(const_iterator first, const_iterator last, const value_type *cstr)](class_luna_1_1_basic_string_1ac785ff9f4e7f00251c2fc902eb6cf00f.md)

    Replaces characters in range [`first`, `last`) with a null-terminated C string. 

* [void replace(usize pos, usize count, usize count2, value_type ch)](class_luna_1_1_basic_string_1aa74f73d93d069eb10f5746467c009cfe.md)

    Replaces characters in range [`pos`, `pos + count`) with `count2` copies of character `ch`. 

* [void replace(const_iterator first, const_iterator last, usize count2, value_type ch)](class_luna_1_1_basic_string_1a861d541f8e33a502bbf985c6bee9e39c.md)

    Replaces characters in range [`first`, `last`) with `count2` copies of character `ch`. 

* [void replace(const_iterator first, const_iterator last, InitializerList< value_type > ilist)](class_luna_1_1_basic_string_1a5a4028436760fb23d593e0c48bc7436a.md)

    Replaces characters in range [`first`, `last`) with characters from the specified initializer list. 

* [BasicString< _Char, _Alloc > substr(usize pos=0, usize count=npos) const](class_luna_1_1_basic_string_1a04b6fefb11a9d480a598c81a0d29e9bb.md)

    Creates a substring of this string. 

* [usize copy(value_type *dst, usize count, usize pos=0) const](class_luna_1_1_basic_string_1a49b5c5c2c2fb221c030699f473a7578c.md)

    Copies a substring [`pos`, `pos + count`) to character string pointed to by `dst`. 

* [BasicString< _Char, _Alloc >::allocator_type get_allocator() const](class_luna_1_1_basic_string_1a8abd645420e7dbfa486b5eff756c97b0.md)

    Gets the allocator of the string. 

* [usize find(const BasicString &str, usize pos=0) const](class_luna_1_1_basic_string_1accbf8d53216f91730aa09611b24384b5.md)

    Finds the first occurrence of the specified character sequence in the string. 

* [usize find(const value_type *s, usize pos, usize count) const](class_luna_1_1_basic_string_1a94d0a547db1d7bd35eab7d2bdde40344.md)

    Finds the first occurrence of the specified character sequence in the string. 

* [usize find(const value_type *s, usize pos=0) const](class_luna_1_1_basic_string_1acf6eab9445892ede4098e9778af4a2d4.md)

    Finds the first occurrence of the specified character sequence in the string. 

* [usize find(value_type ch, usize pos=0) const](class_luna_1_1_basic_string_1a8db62d39b6326c458c383f5c792f90bb.md)

    Finds the first occurrence of the specified character in the string. 

* [usize rfind(const BasicString &str, usize pos=npos) const](class_luna_1_1_basic_string_1a7503833fd0adcf86380c970edcd84afb.md)

    Finds the last occurrence of the specified character sequence in the string. 

* [usize rfind(const value_type *s, usize pos, usize count) const](class_luna_1_1_basic_string_1a8a8f41ef4cfe42a7233e2318c253ac00.md)

    Finds the last occurrence of the specified character sequence in the string. 

* [usize rfind(const value_type *s, usize pos=0) const](class_luna_1_1_basic_string_1a7d3ce44621aabfcbfbf0005b0a0479ac.md)

    Finds the last occurrence of the specified character sequence in the string. 

* [usize rfind(value_type ch, usize pos=npos) const](class_luna_1_1_basic_string_1ab54fbd34cb23148a39defea3b2e1f5ea.md)

    Finds the first occurrence of the specified character in the string. 

