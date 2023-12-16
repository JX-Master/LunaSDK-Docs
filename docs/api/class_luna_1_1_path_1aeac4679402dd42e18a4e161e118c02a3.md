# Luna::Path::is_subpath_of

```c++
bool is_subpath_of(const Path &base) const
```

Checks whether the current path is one subsequent path of the specified base path. 

For example, "/foo/bar" is a subsequent path of "/foo". 

## Parameters
* *in* **base**

    The base path to be checked. 

## Remark
[Path](class_luna_1_1_path.md) A is the subsequent path of B if:1. [Path](class_luna_1_1_path.md) A contains all nodes of B as its prefix path, in the same order as B.

1. If both paths have root names, their root names should be identical. The path flags (absolute/relative, file/directory) are ignored while checking. 

