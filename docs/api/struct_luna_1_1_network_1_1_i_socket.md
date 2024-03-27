# Luna::Network::ISocket
Represents one socket, which is a network communication endpoint. 

```c++
interface Luna::Network::ISocket : public virtual IStream
```

Each socket is associated with a socket address, which consists of an IP address and a port number. Sockets allow for real-time, bi-directional communication between a client and a server, and are used in various protocols like TCP/IP and UDP. 

## Base type
* [IStream](struct_luna_1_1_i_stream.md)
## Member functions
* [virtual opaque_t get_native_handle()=0](struct_luna_1_1_network_1_1_i_socket_1a05e4a79ff545ae21ddebb7d9d3c64bbd.md)

    Gets the native handle of this socket. 

* [virtual RV bind(const SocketAddress &address)=0](struct_luna_1_1_network_1_1_i_socket_1a5f734196e5f9a4b9e8c12de751f55a8b.md)

    Binds one address to this socket, so that it can be used to listen connections from that address. 

* [virtual RV listen(i32 len)=0](struct_luna_1_1_network_1_1_i_socket_1a3c7ea9575d1dec11fa8d4346e7291ffd.md)

    Starts listening for incoming connections. 

* [virtual RV connect(const SocketAddress &address)=0](struct_luna_1_1_network_1_1_i_socket_1ad826ee44f705188a4be46de2399ef1b8.md)

    Connects to the specified host. 

* [virtual R< Ref< ISocket > > accept(SocketAddress &address)=0](struct_luna_1_1_network_1_1_i_socket_1ae3025c307ab17f7cdf15742f3a90fb2a.md)

    Accepts incoming connection attempt on this socket. 

