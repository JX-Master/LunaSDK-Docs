# Luna::load_file_data

```c++
R< Blob > load_file_data(IFile *file)
```

Returns the data in the specified file as a blob object. 



## Parameters
### file
The file to read. 

## Return value
Returns the data of the file. 

## Valid Usage
* `file` must be opened with FileOpenFlag::read flag. 

