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
* [create_new](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3a310252600a249abffe9224a0921f176f.md)
* [open_always](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3a19489a00a74d7c46c7153d749628bbfd.md)
* [open_existing](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3aa200dcd6176417e93be2405188ae7cc9.md)

    Only opens a file when it does exists. If the file does not exist, the call fails with BasicError::not_found. 

* [open_existing_as_new](group___runtime_file_1gga191cbeed882d989eae99623be3fd60d3a2946e7d8e6aa02dab7b39419c0d44e7b.md)
