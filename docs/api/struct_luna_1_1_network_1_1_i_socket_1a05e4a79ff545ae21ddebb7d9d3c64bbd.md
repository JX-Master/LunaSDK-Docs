# Luna::Network::ISocket::get_native_handle

```c++
virtual opaque_t get_native_handle()=0
```

Gets the native handle of this socket. 

On Windows platforms, the returned handle can be reinterpreted to `SOCKET` type. On POSIX platforms, the returned handle can be reinterpreted to `int`, which is the file descriptor of the socket. 

## Return value
Returns the native handle of this socket. 

