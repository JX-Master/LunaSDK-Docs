# Luna::Network::getaddrinfo

```c++
RV getaddrinfo(const c8 *node, const c8 *service, const AddressInfo *hints, Vector< AddressInfo > &result)
```

Gets address from host domain name, or gets port number from service name. 



## Parameters
* *in* **node**

    The host domain name or address string. 

* *in* **service**

    The service decimal port number or service name (like "ftp", "http", etc.). 

* *in* **hints**

    Hints to the type of the information expected to get from this function. This may be `nullptr`. 

* *out* **result**

    The vector to accept query result. Results will be pushed to the back of this vector. Existing elements will not be modified. 

