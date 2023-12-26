# Luna::Vector::insert

```c++
template <typename _InputIt>
auto insert(const_iterator pos, _InputIt first, _InputIt last) -> enable_if_t<!is_integral_v< _InputIt >, iterator >
```

Inserts one range of elements to the vector. 



## Parameters
* *in* **pos**

    The iterator to the position to insert elements. The elements will be inserted before the element pointed by this iterator. This can be `end()`, indicating that the element will be inserted at the end of the vector. 

* *in* **first**

    The iterator to the first element to be inserted. 

* *in* **last**

    The iterator to the one-past-last element to be inserted. 

## Return value
Returns one iterator to the first inserted element. 

## Valid Usage
* If `pos != end()`, `pos` must points to a valid element in the vector. 

