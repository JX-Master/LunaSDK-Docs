# Luna::load_file_data

```c++
R< Blob > load_file_data(IFile *file)
```

Returns the data in the specified file as a blob object. 



## Parameters
* *in* **file**

    The file to read. 

## Return value
Returns the data of the file. 

## Valid Usage
* `file` must be opened with [FileOpenFlag::read](group___runtime_file_1ggaa6e577ca0057e9e199efe810f7876d3daecae13117d6f0584c25a9da6c8f8415e.md) flag. 

