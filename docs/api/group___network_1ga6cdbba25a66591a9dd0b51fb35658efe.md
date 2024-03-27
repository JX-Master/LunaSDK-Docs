# Luna::Network::Protocol

```c++
enum Protocol : u32
{
    unspecified= 0
    icmp
    igmp
    rfcomm
    tcp
    udp
    icmpv6
}
```

Specifies the transmission protocol used by the socket. 

## Options
* [unspecified](group___network_1gga6cdbba25a66591a9dd0b51fb35658efead415f0e30c471dfdd9bc4f827329ef48.md)

    The network protocol is unspecified. The system chooses the most suitable protocol based on `af` and `type` parameters. 

* [icmp](group___network_1gga6cdbba25a66591a9dd0b51fb35658efea1249ce19ef6180e143506b5287be8a7a.md)

    The Internet Control Message Protocol (ICMP). This is a possible value when the `af` parameter is [AddressFamily::unspecified](group___network_1ggae86311d3afd23c05c7abba98dcb3036bad415f0e30c471dfdd9bc4f827329ef48.md), [AddressFamily::ipv4](group___network_1ggae86311d3afd23c05c7abba98dcb3036ba0485728ba5ed6951c7e858af6c1af7c3.md) or [AddressFamily::ipv6](group___network_1ggae86311d3afd23c05c7abba98dcb3036bacc314cbc6ae71c0724390eb450bb969d.md) and the `type` parameter is [SocketType::raw](group___network_1gga8ae7e0c32046eac388477ca632be1642abdd166af3a63f7be696dd17a218a6ffb.md) or [SocketType::unspecified](group___network_1gga8ae7e0c32046eac388477ca632be1642ad415f0e30c471dfdd9bc4f827329ef48.md). 

* [igmp](group___network_1gga6cdbba25a66591a9dd0b51fb35658efeaaf0ae999ec3d398fee7424091b45d947.md)

    The Internet Group Management Protocol (IGMP). This is a possible value when the `af` parameter is [AddressFamily::unspecified](group___network_1ggae86311d3afd23c05c7abba98dcb3036bad415f0e30c471dfdd9bc4f827329ef48.md), [AddressFamily::ipv4](group___network_1ggae86311d3afd23c05c7abba98dcb3036ba0485728ba5ed6951c7e858af6c1af7c3.md) or [AddressFamily::ipv6](group___network_1ggae86311d3afd23c05c7abba98dcb3036bacc314cbc6ae71c0724390eb450bb969d.md) and the `type` parameter is [SocketType::raw](group___network_1gga8ae7e0c32046eac388477ca632be1642abdd166af3a63f7be696dd17a218a6ffb.md) or [SocketType::unspecified](group___network_1gga8ae7e0c32046eac388477ca632be1642ad415f0e30c471dfdd9bc4f827329ef48.md). 

* [rfcomm](group___network_1gga6cdbba25a66591a9dd0b51fb35658efea0f37142f7c400a845bc972288135fe35.md)

    The Bluetooth Radio Frequency Communications (Bluetooth RFCOMM) protocol. This is a possible value when the `af` parameter is [AddressFamily::bluetooth](group___network_1ggae86311d3afd23c05c7abba98dcb3036ba9abfc3fa0a586782b875ee02ad45dcd8.md) and the `type` parameter is [SocketType::stream](group___network_1gga8ae7e0c32046eac388477ca632be1642af7b44cfafd5c52223d5498196c8a2e7b.md). 

* [tcp](group___network_1gga6cdbba25a66591a9dd0b51fb35658efeae20bb202b1d5537b1415e3263a37ed78.md)

    Use Transmission Control Protocol (TCP). This is a possible value when the `af` parameter is [AddressFamily::ipv4](group___network_1ggae86311d3afd23c05c7abba98dcb3036ba0485728ba5ed6951c7e858af6c1af7c3.md) or [AddressFamily::ipv6](group___network_1ggae86311d3afd23c05c7abba98dcb3036bacc314cbc6ae71c0724390eb450bb969d.md) and the `type` parameter is [SocketType::stream](group___network_1gga8ae7e0c32046eac388477ca632be1642af7b44cfafd5c52223d5498196c8a2e7b.md). 

* [udp](group___network_1gga6cdbba25a66591a9dd0b51fb35658efea84864c1fe095359bc9c5ac068e24e781.md)

    Use User Datagram Protocol (UDP). This is a possible value when the `af` parameter is [AddressFamily::ipv4](group___network_1ggae86311d3afd23c05c7abba98dcb3036ba0485728ba5ed6951c7e858af6c1af7c3.md) or [AddressFamily::ipv6](group___network_1ggae86311d3afd23c05c7abba98dcb3036bacc314cbc6ae71c0724390eb450bb969d.md) and the `type` parameter is [SocketType::dgram](group___network_1gga8ae7e0c32046eac388477ca632be1642afbf7c787e5a1bb8634a7639a596aa786.md). 

* [icmpv6](group___network_1gga6cdbba25a66591a9dd0b51fb35658efeab5ffe149ffbc0b170e1384585e35ab0b.md)

    The Internet Control Message Protocol Version 6 (ICMPv6). This is a possible value when the `af` parameter is [AddressFamily::unspecified](group___network_1ggae86311d3afd23c05c7abba98dcb3036bad415f0e30c471dfdd9bc4f827329ef48.md), [AddressFamily::ipv4](group___network_1ggae86311d3afd23c05c7abba98dcb3036ba0485728ba5ed6951c7e858af6c1af7c3.md) or [AddressFamily::ipv6](group___network_1ggae86311d3afd23c05c7abba98dcb3036bacc314cbc6ae71c0724390eb450bb969d.md) and the `type` parameter is [SocketType::raw](group___network_1gga8ae7e0c32046eac388477ca632be1642abdd166af3a63f7be696dd17a218a6ffb.md) or [SocketType::unspecified](group___network_1gga8ae7e0c32046eac388477ca632be1642ad415f0e30c471dfdd9bc4f827329ef48.md). 

