# Luna::BasicString::BasicString

```c++
template <typename _InputIt>
BasicString(_InputIt first, _InputIt last, const allocator_type &alloc=allocator_type())
```

Constructs one string by coping characters from string specified by the iterator range. 



## Parameters
* *in* **first**

    The iterator to the first character to be copied. 

* *in* **last**

    The iterator to the one-past-last character to be copied. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

