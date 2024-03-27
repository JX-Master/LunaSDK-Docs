# Network Errors
## Functions
* [ErrCode not_connected()](group___network_error_1ga00b794b09cad07cd5043af612fac91dd.md)

    The socket is not connected. 

* [ErrCode already_connected()](group___network_error_1ga0aa32f04abf24f10e66881bf53507d17.md)

    The socket is already connected. 

* [ErrCode network_down()](group___network_error_1ga010f44e96dad627e0db8098a57787550.md)

    The network subsystem has failed. 

* [ErrCode address_not_supported()](group___network_error_1gae7006da610b030e728dfd38207fed64c.md)

    The specified address family is not supported by the socket/protocol. 

* [ErrCode address_in_use()](group___network_error_1gaaf893debd5d13b12f4ed16f9bc4b859d.md)

    The speciifed address is already bound to one existing socket. 

* [ErrCode address_not_available()](group___network_error_1ga7e5468e3bb23ee16e0eaf21b42943785.md)

    The requested address is not available. 

* [ErrCode network_reset()](group___network_error_1ga014023e3d4b0dd81eeafba1320a8a2a1.md)

    For a connection-oriented socket, this error indicates that the connection has been broken due to keep-alive activity that detected a failure while the operation was in progress. For a datagram socket, this error indicates that the time to live has expired. 

* [ErrCode connection_refused()](group___network_error_1gacbd5aa275c8ce4f996b9bad2b8953704.md)

    The attempt to connect was forcefully rejected. 

* [ErrCode connection_aborted()](group___network_error_1gab7bf0fbc0af4f226f8b633f2ccd5bc09.md)

    The virtual circuit was terminated due to a time-out or other failure. The application should close the socket as it is no longer usable. 

* [ErrCode connection_reset()](group___network_error_1ga359e108c30b3eae9a93a8eb2ffa7a9ea.md)

    The virtual circuit was reset by the remote side executing a hard or abortive close. The application should close the socket as it is no longer usable. On a UDP-datagram socket, this error would indicate that a previous send operation resulted in an ICMP "Port Unreachable" message. 

* [ErrCode network_unreachable()](group___network_error_1ga068fbfc6a3d977a7781e2d41f1c22e5b.md)

    The network cannot be reached from this host at this time. 

* [ErrCode host_unreachable()](group___network_error_1gaadfb8007d30a079bfc7fbe5a2a2cd2fd.md)

    A socket operation was attempted to an unreachable host. 

* [ErrCode protocol_not_supported()](group___network_error_1gabbb3c76902b80f53cd5eafc4f5c35e96.md)

    The specified protocol is not supported within this address family. 

* [ErrCode host_not_found()](group___network_error_1gab05eec66b5828d0d0bbfea546ecaaa5a.md)

    The specified host cannot be found. 

* [ErrCode service_not_found()](group___network_error_1gae5af812baf24ad8dbeb405e02b64c206.md)

    The service is not supported on the target host with specified socket type. 

