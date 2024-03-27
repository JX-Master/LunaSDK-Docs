# Luna::Network::ISocket::accept

```c++
virtual R< Ref< ISocket > > accept(SocketAddress &address)=0
```

Accepts incoming connection attempt on this socket. 



## Parameters
* *out* **address**

    The assigned address for the accepted connection. 

## Return value
Returns the socket that represents the accepted connection. 

