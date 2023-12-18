# Luna::FileCreationMode

```c++
enum FileCreationMode : u32
{
    create_always= 1
    create_new= 2
    open_always= 3
    open_existing= 4
    open_existing_as_new= 5
}
```

Specifies file creation mmode. 

## Options
* [create_always](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3ab03c6a6956b8e7be9fe2961b5789ea4d.md)

    Always creates a new file and opens it. If the file already exists, the old file content will be discarded and the file is treated as a new empty file. 

* [create_new](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3a310252600a249abffe9224a0921f176f.md)

    Only creates a file and opens it when it does not exist. If the file already exists, the call fails with BasicError::already_exists. 

* [open_always](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3a19489a00a74d7c46c7153d749628bbfd.md)

    Always opens a file. If the file already exists, the file will be open with its data preserved, if the file does not exist, it will be created and opened. 

* [open_existing](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3aa200dcd6176417e93be2405188ae7cc9.md)

    Only opens a file when it does exists. If the file does not exist, the call fails with BasicError::not_found. 

* [open_existing_as_new](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3a2946e7d8e6aa02dab7b39419c0d44e7b.md)

    Only opens a file when it does exists, and discards the file data so the file is treated as a new file. 

