# Luna::Path
A container that contains a sequence of names that describe one path. 

```c++
class Luna::Path
```

[Path](class_luna_1_1_path.md) is one kind of string that describes the location of one node in a hierarchical-based node tree, given that each node in the tree can be identified by a name string. For example, a file path is used to identify a file or folder in the given file system.

[Path](class_luna_1_1_path.md) is designed to be platform-independent and efficient to handle file path related operations. In implementation, the path object does not store the path string directly, but breaks it down to several parts, and stores each part independently. This makes path-related operations very fast and consumes less memory if you need to store lots of paths.

One path is composed by the following components:1. The root name, which usually determines the domain of the path. For example, then volume symbol on Windows (like C:) is one kind of root name.

1. The directory nodes that composes the path. For example, "C:\Games\MyGame\" has root name "C:" and two directory nodes 
"Games" and "MyGame". In file object, every directory node as well as the root name is stored independently as one [Name](class_luna_1_1_name.md)
 object, and they are grouped into one array to form the path sequence.

1. The path flags, see `EPathFlag` for details. Basically, path object uses flags to determine if one path is absolute (if begins with one separator), and if one path represents a directory (if it ends with one separator). This flags are properly set when the path string gets parsed, but it may not be correct. For example, if you parse one path string that represents a directory but does not ends with a separator, the `EPathFlag::directory` will not be set for that path. The path object will not use runtime system calls like `file_attribute` to determine if one path is valid or represents a directory, it is the user's responsibility to check it before using it. 

## Member functions
* [Path()](class_luna_1_1_path_1aaa44fef284bec9041f7eb22b921c6174.md)

    Constructs one empty path. 

* [Path(const String &str)](class_luna_1_1_path_1adbf7e6539b0ad25282e4fb77b92635b4.md)

    Constructs one path by parsing the specified path string. 

* [Path(const String &str, usize pos)](class_luna_1_1_path_1ac74c1bcf917bd1ba67ebda7b6b815068.md)

    Constructs one path by parsing the specified path string with custom starting position. 

* [Path(const String &str, usize pos, usize count)](class_luna_1_1_path_1af0d3e5a420e1e64cf8d5ad2cfad717ee.md)

    Constructs one path by parsing the specified path string with custom starting position and string size. 

* [Path(const c8 *s)](class_luna_1_1_path_1ab2f799b011c22cb3d0ed69097a602354.md)

    Constructs one path by parsing the specified path string. 

* [Path(const c8 *s, usize count)](class_luna_1_1_path_1a93486edb4c1e7673d42c9c45abd487d4.md)

    Constructs one path by parsing the specified path string. 

* [Path(const Path &rhs)](class_luna_1_1_path_1a6f0b65d8220590bc0de51a6f9178db0c.md)

    Constructs one path by moving coping content from another path. 

* [Path(Path &&rhs)](class_luna_1_1_path_1a7ccd7a00a55cd570e29bf063d550cde0.md)

    Constructs one path by moving moving content from another path. 

* [Path & operator=(const String &str)](class_luna_1_1_path_1a1c1b5cd48d55ddc2bf6f6cc636b2115c.md)

    Replaces content of the path by parsing the specified path string. 

* [Path & operator=(const c8 *s)](class_luna_1_1_path_1a6dea008a7b7a36a8360f693219a60342.md)

    Replaces content of the path by parsing the specified path string. 

* [Path & operator=(const Path &rhs)](class_luna_1_1_path_1ab8d46075aaf0f2d24e57f880fe5a2f51.md)

    Replaces content of the path by coping content from another path. 

* [Path & operator=(Path &&rhs)](class_luna_1_1_path_1a6acef455b6bcc678f8844b29dc330c5a.md)

    Replaces content of the path by coping content from another path. 

* [PathFlag flags() const](class_luna_1_1_path_1ae433944abc9fd0a6a7d1f404cabc0161.md)

    Gets the path flags. 

* [PathFlag & flags()](class_luna_1_1_path_1ab3985f073a6cb98ef41ab10a6e6237d6.md)

    Gets the path flags. 

* [void normalize()](class_luna_1_1_path_1acd0de676568888d848beb97dcc53ae47.md)

    Normalizes the path. 

* [String encode(PathSeparator separator=PathSeparator::slash, bool has_root=true) const](class_luna_1_1_path_1adcf25a5902a60521258ccf9f0ebcff23.md)

    Encodes the current path to a string. 

* [void assign(const Path &rhs)](class_luna_1_1_path_1a6ccb12f7e525f5ea56591ab4985f7ffc.md)

    Replaces content of the path by coping content from another path. 

* [void assign(Path &&rhs)](class_luna_1_1_path_1a0b13de52fa02fe7301a3ad19222d1ed5.md)

    Replaces content of the path by coping content from another path. 

* [void assign(const String &str)](class_luna_1_1_path_1aaf3ff431ade941697522db53026aa3d8.md)

    Replaces content of the path by parsing the specified path string. 

* [void assign(const String &str, usize pos)](class_luna_1_1_path_1ab2f0455e08d54d6e9dbd4a222a2501c6.md)

    Replaces content of the path by parsing the specified path string with custom starting position. 

* [void assign(const String &str, usize pos, usize count)](class_luna_1_1_path_1ad78b5b48657110467ac0e2653d6ecca0.md)

    CReplaces content of the path by parsing the specified path string with custom starting position and string size. 

* [void assign(const c8 *s)](class_luna_1_1_path_1a5ce99aa038c83a37e488b30c9b72b264.md)

    Replaces content of the path by parsing the specified path string. 

* [void assign(const c8 *s, usize count)](class_luna_1_1_path_1a07068d47f128b725dbc93964dc48c0ad.md)

    Replaces content of the path by parsing the specified path string. 

* [void assign_relative(const Path &base, const Path &target)](class_luna_1_1_path_1a38f299dc7e0d3750ae0fadeecae24962.md)

    Assigns the content of this path with a new path that if appended to `base` path, creates a path equal to `target` path. 

* [const Name & root() const](class_luna_1_1_path_1a7786a55970b548f907139eb1ba305322.md)

    Gets the path root name. 

* [Name & root()](class_luna_1_1_path_1a93b14a8ea0945ce65496b6ee7373453a.md)

    Gets the path root name. 

* [Name extension() const](class_luna_1_1_path_1a0a50994e226f282875ffd4789a71548e.md)

    Gets the extension name of the path, that is, the name string after the last dot(.) character. 

* [Name filename() const](class_luna_1_1_path_1afefe2b622247530ff0b1b292a33e905f.md)

    Gets the filename of the path, which is the last node in the path excluding extension and the separating dot(`.`). 

* [void replace_extension(const c8 *new_extension)](class_luna_1_1_path_1a5b8ddc45644b88514324f01fc4850c6b.md)

    Replaces the extension. 

* [void replace_extension(const c8 *new_extension, usize count)](class_luna_1_1_path_1a785ace02c15772e6b69c85ac561df3ae.md)

    Replaces the extension. 

* [void append_extension(const c8 *new_extension)](class_luna_1_1_path_1a978e690ac37f02e6e92ceb690d7bc711.md)

    Appends the extension. 

* [void append_extension(const c8 *new_extension, usize count)](class_luna_1_1_path_1ae6cc9015817f77ee7b14831b579765f5.md)

    Appends the extension. 

* [void remove_extension()](class_luna_1_1_path_1aa18422283cee9a92d1de2d05ebd886b8.md)

    Removes the extension. 

* [const_reference at(usize index) const](class_luna_1_1_path_1a27045ce733dd1f9807788ac3c11a491e.md)

    Gets the name node at the specified index. 

* [reference at(usize index)](class_luna_1_1_path_1ae671ac3329f501e4dedb55204c7eef41.md)

    Gets the name node at the specified index. 

* [const_reference operator[](usize index) const](class_luna_1_1_path_1a4ca6742f3a8c0e58359756b0ad7e3026.md)

    Gets the name node at the specified index. 

* [reference operator[](usize index)](class_luna_1_1_path_1a653eb49e972bb8c18143e8dc85c47fd3.md)

    Gets the name node at the specified index. 

* [iterator begin()](class_luna_1_1_path_1ad69bd11391be1a1dba5c8202259664f8.md)

    Gets one iterator to the first name node of the path. 

* [const_iterator begin() const](class_luna_1_1_path_1a29305669b60ca1680752e2fc3592ba99.md)

    Gets one constant iterator to the first name node of the path. 

* [const_iterator cbegin() const](class_luna_1_1_path_1a39112ae08f6ffc7ee58c6aa79772e094.md)

    Gets one constant iterator to the first name node of the path. 

* [iterator end()](class_luna_1_1_path_1acad38d52497a975bfb6f2f6acd76631f.md)

    Gets one iterator to the one past last name node of the path. 

* [const_iterator end() const](class_luna_1_1_path_1accf9a4bd0c34d4a5f6a7dab66ea10cdc.md)

    Gets one constant iterator to the one past last name node of the path. 

* [const_iterator cend() const](class_luna_1_1_path_1a93791e61ab486b4022c389d634b4facc.md)

    Gets one constant iterator to the one past last name node of the path. 

* [reverse_iterator rbegin()](class_luna_1_1_path_1acea44ed500a54b2bb93e16b86e81afa8.md)

    Gets one reverse iterator to the last name node of the path. 

* [const_reverse_iterator rbegin() const](class_luna_1_1_path_1af086cceac199bd735c7a97c2a8d7ed21.md)

    Gets one constant reverse iterator to the last name node of the path. 

* [const_reverse_iterator crbegin() const](class_luna_1_1_path_1a81f80a31923e85af56a7b1ae0712a33b.md)

    Gets one constant reverse iterator to the last name node of the path. 

* [reverse_iterator rend()](class_luna_1_1_path_1a68c599ddcbfddc65170de524ac165e44.md)

    Gets one reverse iterator to the one-before-first name node of the path. 

* [const_reverse_iterator rend() const](class_luna_1_1_path_1a07da1fdc890b6949f1a20a1961c6fc44.md)

    Gets one constant reverse iterator to the one-before-first name node of the path. 

* [const_reverse_iterator crend() const](class_luna_1_1_path_1abef9dfc7607c7e1a3854788ba56a4f34.md)

    Gets one constant reverse iterator to the one-before-first name node of the path. 

* [usize size() const](class_luna_1_1_path_1a79348f1b7c06b34052b42656a0279429.md)

    Gets the size of the path, that is, the number of name nodes in the path. 

* [bool empty() const](class_luna_1_1_path_1a644718bb2fb240de962dc3c9a1fdf0dc.md)

    Checks whether this path is empty, that is, the size of this path is `0`. 

* [reference front()](class_luna_1_1_path_1a6a48363b4355f6f5b441637774f79a59.md)

    Gets the first name node in the path. 

* [const_reference front() const](class_luna_1_1_path_1a0ae6b4f9719202f7ddb334c16fb03d80.md)

    Gets the first name node in the path. 

* [reference back()](class_luna_1_1_path_1af71e6c1eccbc12e9339c00a86a981a43.md)

    Gets the last name node in the path. 

* [const_reference back() const](class_luna_1_1_path_1a61772c77ad2abfbb296912e7281e154c.md)

    Gets the last name node in the path. 

* [void push_back(const Name &path_node)](class_luna_1_1_path_1acb0ff70a20d6bb5ea56b8c5c9a5c198b.md)

    Inserts one name node at the back of the path. 

* [void push_back(Name &&path_node)](class_luna_1_1_path_1abe4510c91d51327a875596eac8c238b6.md)

    Inserts one name node at the back of the path. 

* [void pop_back()](class_luna_1_1_path_1a058bda4957df6a97b1ea6c9fd783f672.md)

    Removes the last name node of the path. 

* [void append(const Path &appended_path)](class_luna_1_1_path_1a79bc3eff38f18e90af46526dd4595a4b.md)

    Appends another path to the end of this path. 

* [void append(const Path &appended_path, usize pos)](class_luna_1_1_path_1af6073c5186c21acacde749524f8084a6.md)

    Appends another path to the end of this path. 

* [void append(const Path &appended_path, usize pos, usize count)](class_luna_1_1_path_1aeb65295a550d14c73c933be870a9412e.md)

    Appends another path to the end of this path. 

* [void clear()](class_luna_1_1_path_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Clears all nodes in the path. 

* [void reset()](class_luna_1_1_path_1ad20897c5c8bd47f5d4005989bead0e55.md)

    Resets the path object. 

* [iterator erase(const_iterator pos)](class_luna_1_1_path_1a29790c28710ec0e64b48c2f4edd0b08c.md)

    Removes one name node from the path. 

* [iterator erase(const_iterator first, const_iterator last)](class_luna_1_1_path_1aa3af768723cd533218ea3d83af440713.md)

    Removes one range of name nodes from the path. 

* [usize hash_code() const](class_luna_1_1_path_1aa4d2e3f76cdd763239847613176226fc.md)

    Computes the hash code of this path. 

* [bool is_subpath_of(const Path &base) const](class_luna_1_1_path_1aeac4679402dd42e18a4e161e118c02a3.md)

    Checks whether the current path is one subsequent path of the specified base path. 

* [bool equal_to(const Path &rhs, PathComponent compared_components=PathComponent::all) const](class_luna_1_1_path_1a2c04c06788cea21fabc550d98791986b.md)

    Compares two paths for equality. 

* [bool operator==(const Path &rhs) const](class_luna_1_1_path_1aa3f7adcb8eaf8e0b1288c248bbb035a8.md)

    Compares all components of two paths for equality. 

* [bool operator!=(const Path &rhs) const](class_luna_1_1_path_1a30239146566a281f5112902a0a47634e.md)

    Compares all components of two paths for non-equality. 

