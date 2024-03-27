# Network
Network module provides uniform socket-based APIs to access platform's network features. 

## Topics
* [Network Errors](network_error.md)
## Types
* [Luna::Network::IPv4Address](struct_luna_1_1_network_1_1_i_pv4_address.md)

    Specifies one IPv4 address. 


* [Luna::Network::IPv6Address](struct_luna_1_1_network_1_1_i_pv6_address.md)

    Specifies one IPv6 address. 


* [Luna::Network::SocketAddressIPv4](struct_luna_1_1_network_1_1_socket_address_i_pv4.md)

    The address to use when opening a socket using IPv4 address. 


* [Luna::Network::SocketAddress](struct_luna_1_1_network_1_1_socket_address.md)

    Specifies address to use when opening a socket. 


* [Luna::Network::ISocket](struct_luna_1_1_network_1_1_i_socket.md)

    Represents one socket, which is a network communication endpoint. 


* [Luna::Network::AddressInfo](struct_luna_1_1_network_1_1_address_info.md)

    The address information fetched from [getaddrinfo](group___network_1gaf2238fdd2026bbc1af23c63151fe75a8.md). 


## Enumerations
* [Luna::Network::AddressFamily](group___network_1gae86311d3afd23c05c7abba98dcb3036b.md)

    Specifies address family. 

* [Luna::Network::SocketType](group___network_1ga8ae7e0c32046eac388477ca632be1642.md)

    Specifies the socket type. 

* [Luna::Network::Protocol](group___network_1ga6cdbba25a66591a9dd0b51fb35658efe.md)

    Specifies the transmission protocol used by the socket. 

* [Luna::Network::AddressInfoFlag](group___network_1ga37884001db7201b0d1e6a781738e729f.md)

    Specifies flag attributes of one address. 

## Constants
* [constexpr IPv4Address IPV4_ADDRESS_ANY](group___network_1ga28ea193f9e4eba70aff32026118f2e6a.md)

    A special IPv4 address that does not specify any particular address. 

## Functions
* [u32 hton(u32 hostlong)](group___network_1gab89066043f4615c1531e722a5b940c88.md)

    Converts one unsigned integer from host byte order to network byte order. 

* [u16 hton(u16 hostshort)](group___network_1gae58337314dd0cf846e0a68e079947759.md)

    Converts one unsigned short integer from host byte order to network byte order. See remarks of [hton](group___network_1gab89066043f4615c1531e722a5b940c88.md) for details. 

* [u32 ntoh(u32 netlong)](group___network_1ga1e9bedb4f9afa66d535c9e4bbc9a5e2a.md)

    Converts one unsigned integer from network byte order to host byte order. See remarks of [hton](group___network_1gab89066043f4615c1531e722a5b940c88.md) for details. 

* [u16 ntoh(u16 netshort)](group___network_1ga8b12d6b388cfbeb7f681f81ff9aaf6b4.md)

    Converts one unsigned short integer from network byte order to host byte order. See remarks of [hton](group___network_1gab89066043f4615c1531e722a5b940c88.md) for details. 

* [R< Ref< ISocket > > new_socket(AddressFamily af, SocketType type, Protocol protocol)](group___network_1ga79af59361ec21058eb883c3f54df48d0.md)

    Creates one new socket. 

* [RV getaddrinfo(const c8 *node, const c8 *service, const AddressInfo *hints, Vector< AddressInfo > &result)](group___network_1gaf2238fdd2026bbc1af23c63151fe75a8.md)

    Gets address from host domain name, or gets port number from service name. 

