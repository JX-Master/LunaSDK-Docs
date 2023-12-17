# Luna::FileOpenFlag::user_buffering

```c++
user_buffering = 0x04
```

Allocates one user-mode buffer for the opened file. The user-mode buffer can be used to buffer the data read from file or to be written to file, thus reduce system calls if lots of small-sized reads/writes need to be performed. 

