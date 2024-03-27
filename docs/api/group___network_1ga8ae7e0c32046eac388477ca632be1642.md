# Luna::Network::SocketType

```c++
enum SocketType : u32
{
    unspecified= 0
    stream
    dgram
    raw
    rdm
}
```

Specifies the socket type. 

## Options
* [unspecified](group___network_1gga8ae7e0c32046eac388477ca632be1642ad415f0e30c471dfdd9bc4f827329ef48.md)

    The socket type is unspecified. 

* [stream](group___network_1gga8ae7e0c32046eac388477ca632be1642af7b44cfafd5c52223d5498196c8a2e7b.md)

    Maps to `SOCK_STREAM` Provides sequenced, reliable, two-way, connection-based byte streams. 
 An out-of-band data transmission mechanism may be supported. 

* [dgram](group___network_1gga8ae7e0c32046eac388477ca632be1642afbf7c787e5a1bb8634a7639a596aa786.md)

    Maps to `SOCK_DGRAM` Supports datagrams (connectionless, unreliable messages of a fixed maximum length). 

* [raw](group___network_1gga8ae7e0c32046eac388477ca632be1642abdd166af3a63f7be696dd17a218a6ffb.md)

    Maps to `SOCK_RAW` Provides raw network protocol access. 

* [rdm](group___network_1gga8ae7e0c32046eac388477ca632be1642a4625809eb2690f70abd21c4a9aa6b2c7.md)

    Maps to `SOCK_RDM` Provides a reliable datagram layer that does not guarantee ordering. 

