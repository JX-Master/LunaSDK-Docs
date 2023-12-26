# Luna::Span
Represents one reference to one continuous sequence of instances. The size of the span is fixed and specified as template argument. 

```c++
template <typename _Ty, usize _Size>
class Luna::Span
```

## Member functions
* [constexpr Span()](class_luna_1_1_span_1a8d068f5faac74fa3f3c35bbf7720383d.md)

    Constructs one empty span. 

* [constexpr Span(element_type *arr)](class_luna_1_1_span_1a7c5cb706d081a76b786cb1dc81cd4cc2.md)

    Constructs one span by providing the referred range directly. 

* [constexpr Span(InitializerList< remove_cv_t< _Ty > > ilist)](class_luna_1_1_span_1a64585f3aab513db8e318eaacdea37aaa.md)

    Constructs one span using the data provided by the specified initializer list. 

* [constexpr Span(const Span &rhs)=default](class_luna_1_1_span_1a60d0e59b8ec078ea87333f5b6219b791.md)

    Constructs one span by coping data from another span. 

* [constexpr Span & operator=(const Span &rhs)=default](class_luna_1_1_span_1a6dd33e81ac42ce4c7fbe4bb9a3e53b07.md)

    Assigns one span by coping data from another span. 

* [constexpr iterator begin() const](class_luna_1_1_span_1ad6b612835d1d31f5de4de170810bdce1.md)

    Gets one iterator to the first element of the span. 

* [constexpr iterator end() const](class_luna_1_1_span_1abaef5f7fc8ca1254e8ecd8554f0383c9.md)

    Gets one iterator to the one past last element of the span. 

* [constexpr reverse_iterator rbegin() const](class_luna_1_1_span_1a6eb197430bcfe5f252645ef622d2f527.md)

    Gets one reverse iterator to the last element of the span. 

* [constexpr reverse_iterator rend() const](class_luna_1_1_span_1aa7e1a84f0be016a585ede27c006ca37d.md)

    Gets one reverse iterator to the one-before-first element of the span. 

* [constexpr reference front() const](class_luna_1_1_span_1ada7549faa8cde6cb3ed467550cc01233.md)

    Gets a reference to the first (index 0) element in the span. 

* [constexpr reference back() const](class_luna_1_1_span_1a04dd6cf78d02c2011673cf2046720b8e.md)

    Gets a reference to the last (index `size()` - 1) element in the span. 

* [constexpr reference operator[](usize index) const](class_luna_1_1_span_1afefa2aa6ac0e04fc3f8292582a3d9362.md)

    Gets a refernece of the element at the specified index. 

* [constexpr pointer data() const](class_luna_1_1_span_1af4c79a978fadf42753f0034c4d3a3e5c.md)

    Gets one pointer to the span data memory. 

* [constexpr usize size() const](class_luna_1_1_span_1adb59c183f075f048ae90778d15189686.md)

    Gets the size (number of elements) of the span. 

* [constexpr usize size_bytes() const](class_luna_1_1_span_1aebe478efcbe0a2465e4a605594dd8ca0.md)

    Gets the size of the span in bytes, which is `size() * sizeof(element_type)`. 

* [constexpr bool empty() const](class_luna_1_1_span_1afaafdfc441c2433c70959e3dfe46fd97.md)

    Checks whether this span is empty, that is, the size of this span is `0`. 

* [constexpr Span< element_type, _Count > first() const](class_luna_1_1_span_1a5ab239c213ff8a775d6d5f14dea7d9de.md)

    Creates a new fixed-sized span referring the first `_Count` elements of this span. 

* [constexpr Span< element_type, DYNAMIC_EXTENT > first(usize count) const](class_luna_1_1_span_1aa1c5f72b31d5f62bcc96bd2f05c4ef56.md)

    Creates a new dynamic-sized span referring the first `count` elements of this span. 

* [constexpr Span< element_type, _Count > last() const](class_luna_1_1_span_1a8eea75165d56f1e11ee6ce7e693093c1.md)

    Creates a new fixed-sized span referring the last `_Count` elements of this span. 

* [constexpr Span< element_type, DYNAMIC_EXTENT > last(usize count) const](class_luna_1_1_span_1add30b62e5d676d91fe4bc7d72da55683.md)

    Creates a new dynamic-sized span referring the last `count` elements of this span. 

* [constexpr Span< element_type, _Count > subspan(usize offset) const](class_luna_1_1_span_1ac48c9e3eeddf0fc993b947ae0dc900f0.md)

    Creates a new fixed-sized span referring `_Count` elements beginning at `offset` of this span. 

* [constexpr Span< element_type, DYNAMIC_EXTENT > subspan(usize offset, usize count) const](class_luna_1_1_span_1a3d591b31f09473a778716126837d0f9e.md)

    Creates a new dynamic-sized span referring `count` elements beginning at `offset` of this span. 

