# Luna::NetworkError::connection_reset

```c++
ErrCode connection_reset()
```

The virtual circuit was reset by the remote side executing a hard or abortive close. The application should close the socket as it is no longer usable. On a UDP-datagram socket, this error would indicate that a previous send operation resulted in an ICMP "Port Unreachable" message. 

