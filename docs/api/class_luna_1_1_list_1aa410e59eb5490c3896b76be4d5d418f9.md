# Luna::List::sort

```c++
template <typename _Compare>
void sort(_Compare comp)
```

Sorts elements in using the user-specified comparison function object. 



## Parameters
### comp
The comparison function object to use. 

#### Valid Usage
* `comp` must provide the following function: `bool operator()(const _Ty& a, const _Ty& b)`, that returns `true` if `a` should appear in the list before `b`. 

