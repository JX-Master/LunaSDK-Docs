# Luna::find

```c++
template <typename _InputIt, typename _Ty>
constexpr _InputIt find(_InputIt first, _InputIt last, const _Ty &value)
```

Searches for the first element in the range that is equal to (==) the specified value. 



## Parameters
* *in* **first**

    The iterator to the first element of the search range. 

* *in* **last**

    The iterator to the one-past-last element of the search range. 

* *in* **value**

    The value to compare for equality. 

## Return value
Returns one iterator to the first element that is equal to the specified value. Returns `last` if not found. 

