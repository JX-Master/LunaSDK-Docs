# Algorithms
## Functions
* [constexpr const _Ty & min(const _Ty &a, const _Ty &b)](group___runtime_algorithm_1ga147659ad95276a9b14825c4c2452bce6.md)

    Returns the smaller of the given values. 

* [constexpr const _Ty & min(const _Ty &a, const _Ty &b, _LessComp less_comp)](group___runtime_algorithm_1ga3a8ea741d7e44683b3f90bf71fced6fa.md)

    Returns the smaller of the given values. 

* [constexpr const _Ty & max(const _Ty &a, const _Ty &b)](group___runtime_algorithm_1ga44f147d1f9a010b109bf59872d327e38.md)

    Returns the greater of the given values. 

* [constexpr const _Ty & max(const _Ty &a, const _Ty &b, _LessComp less_comp)](group___runtime_algorithm_1gae0f2d82171f4e735f6c9c667ca4c61dd.md)

    Returns the greater of the given values. 

* [void swap(_Ty &a, _Ty &b)](group___runtime_algorithm_1gab9f335c1db01662355d08c95f82d1d24.md)

    Swaps two values. 

* [bool equal(_Iter1 first1, _Iter1 last1, _Iter2 first2)](group___runtime_algorithm_1ga622971e5f7d0e413ef3941c6092d7849.md)

    Tests the equality of two ranges. 

* [bool equal(_Iter1 first1, _Iter1 last1, _Iter2 first2, _EqualComp equal_compare)](group___runtime_algorithm_1ga0391eb9b8b2b28284c625b1e51f02813.md)

    Tests the equality of two ranges. 

* [auto search(_ForwardIt first, _ForwardIt last, _ForwardIt pattern_first, _ForwardIt pattern_last) -> enable_if_t< is_pointer_v< _ForwardIt >, _ForwardIt >](group___runtime_algorithm_1ga91f5e4923dec9e86dc7898acf96f9d4e.md)

    Searches for the first occurrence of the sequence of elements in the specified range. 

* [auto find_end(_ForwardIt first, _ForwardIt last, _ForwardIt pattern_first, _ForwardIt pattern_last) -> enable_if_t< is_pointer_v< _ForwardIt >, _ForwardIt >](group___runtime_algorithm_1gaa7d4ef4a1201800ca9187591a73faba6.md)

    Searches for the last occurrence of the sequence of elements in the specified range. 

* [constexpr _InputIt find(_InputIt first, _InputIt last, const _Ty &value)](group___runtime_algorithm_1ga5c427ac4e48338499c50b6fbffed62bd.md)

    Searches for the first element in the range that is equal to (==) the specified value. 

* [constexpr _InputIt find_if(_InputIt first, _InputIt last, _UnaryPredicate p)](group___runtime_algorithm_1gae5453bc4d172c9055454c73fb47150d9.md)

    Searches for the first element in the range that passes the user-provided unary predicate. 

* [constexpr _InputIt find_if_not(_InputIt first, _InputIt last, _UnaryPredicate q)](group___runtime_algorithm_1gacd42dbba4eb002d62aba4a5e73136c1a.md)

    Searches for the first element in the range that fails the user-provided unary predicate. 

* [constexpr bool all_of(_InputIt first, _InputIt last, _UnaryPredicate p)](group___runtime_algorithm_1gaeb67b9af6950f0144ee3940274a2f586.md)

    Checks if the unary predicate returns `true` for all elements in the range. 

* [constexpr bool any_of(_InputIt first, _InputIt last, _UnaryPredicate p)](group___runtime_algorithm_1ga4d6ea50d77bcca151eae75c7e9f5e9ff.md)

    Checks if the unary predicate returns `true` for at least one element in the range. 

* [constexpr bool none_of(_InputIt first, _InputIt last, _UnaryPredicate p)](group___runtime_algorithm_1gaa2e088af2e0c50dd41eccda423ad419b.md)

    Checks if the unary predicate returns `false` for all elements in the range. 

* [constexpr _UnaryFunction for_each(_InputIt first, _InputIt last, _UnaryFunction f)](group___runtime_algorithm_1gaec62c07d494fde510ad4bc6a4421b51c.md)

    Applies the given function object to every element in the range, in order. 

* [void sort(_RandomIt first, _RandomIt last)](group___runtime_algorithm_1gac1955e41a312fe40f9795a44a51cb4cf.md)

    Sorts the elements in the range in non-descending order. The order of equal elements is not guaranteed to be preserved. 

* [void sort(_RandomIt first, _RandomIt last, _Compare comp)](group___runtime_algorithm_1gaf79ba68237591937a91d96e1ef807944.md)

    Sorts the elements in the range in non-descending order. The order of equal elements is not guaranteed to be preserved. 

* [_ForwardIt upper_bound(_ForwardIt first, _ForwardIt last, const _Ty &value)](group___runtime_algorithm_1ga1f8fc6922e9b20976056dec2d59b89cc.md)

    Finds the first element in the range such that `value < element` is `true`. 

* [_ForwardIt upper_bound(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)](group___runtime_algorithm_1ga8585025fd99a8ee19f11a8ad16ccb15b.md)

    Finds the first element in the range such that `comp(value, element)` is `true`. 

* [_ForwardIt lower_bound(_ForwardIt first, _ForwardIt last, const _Ty &value)](group___runtime_algorithm_1gadb4722898f14cc14eca45afc0affe514.md)

    Finds the first element in the range such that `element < value` is `false`. 

* [_ForwardIt lower_bound(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)](group___runtime_algorithm_1ga6ac8c4d3198b4604c7a091ed93521b48.md)

    Finds the first element in the range such that `comp(element, value)` is `false`. 

* [bool binary_search(_ForwardIt first, _ForwardIt last, const _Ty &value)](group___runtime_algorithm_1ga56e90c79b7400e2bbff7b2fc7e0baf1d.md)

    Checks if an element equivalent to the specified value appears within the range. 

* [bool binary_search(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)](group___runtime_algorithm_1gae17af06dbbf1ba7013de2b4ca50783d5.md)

    Checks if an element equivalent to the specified value appears within the range. 

* [_ForwardIt binary_search_iter(_ForwardIt first, _ForwardIt last, const _Ty &value)](group___runtime_algorithm_1ga9780e6b83d6b4e4c2a8fb6f1195daf2d.md)

    Finds an element equivalent to the specified value in the range. 

* [_ForwardIt binary_search_iter(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)](group___runtime_algorithm_1ga0ad37076ea35bbf85db8b16099e57f5a.md)

    Finds an element equivalent to the specified value in the range. 

* [Pair< _ForwardIt, _ForwardIt > equal_range(_ForwardIt first, _ForwardIt last, const _Ty &value)](group___runtime_algorithm_1ga53e062c1f9ef3170e738a71ea756a7bd.md)

    Gets a range containing all elements equivalent to the specified value in the range. 

* [Pair< _ForwardIt, _ForwardIt > equal_range(_ForwardIt first, _ForwardIt last, const _Ty &value, _Compare comp)](group___runtime_algorithm_1gaf65d96a5a322fb0ed174cda6b3de8847.md)

    Gets a range containing all elements equivalent to the specified value in the range. 

* [bool includes(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2)](group___runtime_algorithm_1gab776c0c36632ba15f2b8637f4aa18b16.md)

    Checks if the sorted range [`first2`, `last2`) is a subsequence of the sorted range [`first1`, `last1`). (A subsequence need not be contiguous.) 

* [bool includes(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _Compare comp)](group___runtime_algorithm_1ga5f2487857061fcf0a115c13a476a1222.md)

    Checks if the sorted range [`first2`, `last2`) is a subsequence of the sorted range [`first1`, `last1`). (A subsequence need not be contiguous.) 

* [_OutputIt copy(_InputIt first, _InputIt last, _OutputIt d_first)](group___runtime_algorithm_1ga82c4c36785b5acdc4d4f8a702b949660.md)

    Copies elements from one range to another range. 

* [_OutputIt copy_if(_InputIt first, _InputIt last, _OutputIt d_first, UnaryPredicate pred)](group___runtime_algorithm_1gac9ec916bcbe424ac468c46772bb94605.md)

    Copies elements that pass user-defined function from one range to another range. The relative order of elements that are copied is preserved. 

* [_OutputIt set_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first)](group___runtime_algorithm_1ga7f57a6a6498420c062c1af9141080b17.md)

    Copies elements that appear in the first sorted range and do not appear in the second sorted range to the destination range. The destination range is also sorted. 

* [_OutputIt set_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first, _Compare comp)](group___runtime_algorithm_1gad5b157c8d26251a7520da620b9434554.md)

    Copies elements that appear in the first sorted range and do not appear in the second sorted range to the destination range. The destination range is also sorted. 

* [_OutputIt set_intersection(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first)](group___runtime_algorithm_1ga6c2f327e87aecc5de9593f6b4b2807ce.md)

    Constructs a sorted range consisting of elements that are found in both sorted ranges. 

* [_OutputIt set_intersection(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first, _Compare comp)](group___runtime_algorithm_1gaf546e5c4c399943badebda3ff2f355c0.md)

    Constructs a sorted range consisting of elements that are found in both sorted ranges. 

* [_OutputIt set_symmetric_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first)](group___runtime_algorithm_1ga4902d63e5b5d907172734ff3ec4a2adf.md)

    Computes symmetric difference of two sorted ranges: elements that are found in either of the ranges, but not in both of them are copied to the destination range. The destination range is also sorted. 

* [_OutputIt set_symmetric_difference(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first, _Compare comp)](group___runtime_algorithm_1ga556703289c68c3e7548657f42807a9a3.md)

    Computes symmetric difference of two sorted ranges: elements that are found in either of the ranges, but not in both of them are copied to the destination range. The destination range is also sorted. 

* [_OutputIt set_union(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first)](group___runtime_algorithm_1ga52881ea0d7864b4201d5c34a9f65e975.md)

    Constructs a sorted union beginning at the destination range consisting of the set of elements present in one or both sorted ranges. 

* [_OutputIt set_union(_InputIt1 first1, _InputIt1 last1, _InputIt2 first2, _InputIt2 last2, _OutputIt d_first, _Compare comp)](group___runtime_algorithm_1ga69dd3d53c2eb4f49fefa002b643e3231.md)

    Constructs a sorted union beginning at the destination range consisting of the set of elements present in one or both sorted ranges. 

