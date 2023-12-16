# Luna::Path::assign

```c++
void assign(const String &str)
```

Replaces content of the path by parsing the specified path string. 



## Parameters
* *in* **str**

    The path string. 

## Remark
Currently only the following root string will be recognized:* Windows volume: C:, D: etc.

* Remove Server: //My_Server or \My_Server or IP-address format(\192.168.31.1) 

