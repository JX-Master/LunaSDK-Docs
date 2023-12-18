# Luna::Span::subspan

```c++
template <usize>
constexpr Span< element_type, _Count > subspan(usize offset) const
```

Creates a new fixed-sized span referring `_Count` elements beginning at `offset` of this span. 



## Parameters
* *in* **offset**

    The index of the first element to refer for the new span. 

## Return value
Returns one span referring `_Count` elements beginning at `offset` of this span. 

