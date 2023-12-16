# Luna::ReverseIterator
An iterator adaptor that reverses the direction of a given iterator. 

```c++
class Luna::ReverseIterator
```

The given iterator must be at least an bidirectional iterator. 

## Member functions
* [constexpr ReverseIterator()](class_luna_1_1_reverse_iterator_1a7a27a93824c22c3d1062eda8f36bf9b0.md)

    Constructs an empty reverse iterator. 

* [constexpr ReverseIterator(iterator_type i)](class_luna_1_1_reverse_iterator_1a262df38391f7cebfd071a522a744ba4a.md)

    Constructs a reverse iterator for the given iterator. 

* [constexpr ReverseIterator(const ReverseIterator &ri)](class_luna_1_1_reverse_iterator_1a07f9fc974b732184a91f03d404cf38e5.md)

    Constructs a reverse iterator by coping from the specified reverse iterator. 

* [constexpr ReverseIterator(const ReverseIterator< _Uty > &ri)](class_luna_1_1_reverse_iterator_1a880cf7ee1debad9672e00064d6bb5228.md)

    Constructs a reverse iterator by coping from the specified reverse iterator of different iterator type. 

* [constexpr iterator_type base() const](class_luna_1_1_reverse_iterator_1a400de181c195ee419fecece2689d44cc.md)

    Gets the base iterator of this reverse iterator. 

* [constexpr reference operator*() const](class_luna_1_1_reverse_iterator_1abae71b38b2deccb8c7b6956db40cf670.md)

    Gets the object this iterator points to. 

* [constexpr pointer operator->() const](class_luna_1_1_reverse_iterator_1adce875cdb45f3fb34643b8a8bfe9e258.md)

    Gets one pointer to the object this iterator points to. 

* [constexpr ReverseIterator & operator++()](class_luna_1_1_reverse_iterator_1a04c10267229369040999255d87aa3a7e.md)

    Pre-increments the iterator to the next object, which is the last object the base iterator points to. 

* [constexpr ReverseIterator operator++(int)](class_luna_1_1_reverse_iterator_1a05aba67cbe324325ac708d6694b1baa0.md)

    Post-increments the iterator to the next object, which is the last object the base iterator points to. 

* [constexpr ReverseIterator & operator--()](class_luna_1_1_reverse_iterator_1a462221ea988ebbbf625cdfd6defaa348.md)

    Pre-decrements the iterator to the last object, which is the next object the base iterator points to. 

* [constexpr ReverseIterator operator--(int)](class_luna_1_1_reverse_iterator_1acec6c1dc8f0d6f87c794808f19f87396.md)

    Post-decrements the iterator to the last object, which is the next object the base iterator points to. 

* [constexpr ReverseIterator operator+(isize n) const](class_luna_1_1_reverse_iterator_1ad383851db942340c7eada562c5977bbb.md)

    Gets one iterator which is advanced by `n` positions respectively. 

* [constexpr ReverseIterator & operator+=(isize n)](class_luna_1_1_reverse_iterator_1a2898cb2d3fc27522131b180bb878dd28.md)

    Advances the iterator by `n` positions respectively. 

* [constexpr ReverseIterator operator-(isize n) const](class_luna_1_1_reverse_iterator_1afc07350a9d4a009150e92c972423e297.md)

    Gets one iterator which is advanced by `-n` positions respectively. 

* [constexpr ReverseIterator & operator-=(isize n)](class_luna_1_1_reverse_iterator_1a28a5b5ae737fec33586d3751a67d4c7f.md)

    Advances the iterator by `-n` positions respectively. 

* [constexpr reference operator[](isize n) const](class_luna_1_1_reverse_iterator_1a28b609b37d166f341abde3197efe2b2a.md)

    Returns a reference to the element at specified relative location. 

