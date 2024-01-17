# Runtime
The Runtime module provides the runtime environment of Luna SDK and defines core functionalities that will be used by almost all modules. 

## Topics
* [Algorithms](runtime_algorithm.md)
* [Containers](runtime_container.md)
* [Assertions](runtime_assert.md)
* [Atomic Operations](runtime_atomic.md)
* [Basic types](runtime_base_type.md)
* [Base64 encoding/decoding](runtime_base64.md)
* [Base85 encoding/decoding](runtime_base85.md)
* [Debugging](runtime_debug.md)
* [DLL loading](runtime_d_l_l.md)
* [Error handling](runtime_error.md)
* [Files](runtime_file.md)
* [Hashing functions](runtime_hash.md)
* [Interfaces](runtime_interface.md)
* [Logging](runtime_log.md)
* [Math library](runtime_math.md)
* [Memory allocation and deallocation](runtime_memory.md)
* [Memory utility library](runtime_memory_utils.md)
* [Module system](runtime_module.md)
* [Name strings](runtime_name.md)
* [Boxed objects](runtime_object.md)
* [Path](runtime_path.md)
* [Debugging](runtime_profiler.md)
* [Generating random numbers](runtime_random.md)
* [SDK initialization and shutdown](runtime_init.md)
* [Serialization](runtime_serialization.md)
* [String library](runtime_string.md)
* [Thread management and synchronization methods](runtime_thread.md)
* [Times](runtime_time.md)
* [Thread safe assertion](runtime_t_s_assert.md)
* [Type reflection](runtime_type.md)
* [Unicode encoding/decoding](runtime_unicode.md)
## Types
* [Luna::Allocator](class_luna_1_1_allocator.md)

    The default allocator implementation that can be used for allocating memory for containers defined in Runtime module. 


* [Luna::Blob](class_luna_1_1_blob.md)

    Represents one binary large object (BLOB). 


* [Luna::Event](class_luna_1_1_event.md)

    Represents one event that once triggered, invokes all handlers registered to it. 


* [Luna::equal_to](struct_luna_1_1equal__to.md)

    Function object for performing comparisons. Unless specialised, invokes `operator==` on type T. 


* [Luna::less](struct_luna_1_1less.md)

    Function object for performing comparisons. Unless specialized, invokes `operator<` on type T. 


* [Luna::hash](struct_luna_1_1hash.md)

    Function object that hashes the specified type into a `usize` hash code that can be used in hash map and hash set. 


* [Luna::ReferenceWrapper](class_luna_1_1_reference_wrapper.md)

    Wraps one reference to one copyable, assignable object. 


* [Luna::Function< _R(_Args...)>](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4.md)

    A function wrapper that can store one callable object, and enable coping, moving and invoking of such callable object. 


* [Luna::ReverseIterator](class_luna_1_1_reverse_iterator.md)

    An iterator adaptor that reverses the direction of a given iterator. 


* [Luna::ObjRef](class_luna_1_1_obj_ref.md)

    The smart pointer that represents one typeless strong reference to one boxed object. 


* [Luna::Ref](class_luna_1_1_ref.md)

    The smart pointer that represents one typed strong reference to one boxed object. 


* [Luna::WeakObjRef](class_luna_1_1_weak_obj_ref.md)

    The smart pointer that represents one typeless weak reference to one boxed object. 


* [Luna::WeakRef](class_luna_1_1_weak_ref.md)

    The smart pointer that represents one typed weak reference to one boxed object. 


* [Luna::IStream](struct_luna_1_1_i_stream.md)

    Represents a serial stream sequence of bytes and supports read/write operations on them. 


* [Luna::ISeekableStream](struct_luna_1_1_i_seekable_stream.md)

    Represents one stream object that supports setting the cursor position. 


* [Luna::Tuple](class_luna_1_1_tuple.md)

    Represents a sequence of fixed-size elements. Every element can have one different type. 


* [Luna::DefaultDelete](struct_luna_1_1_default_delete.md)

    The default object deletion function used by [UniquePtr](class_luna_1_1_unique_ptr.md), which calls [memdelete](group___runtime_memory_1gaf95818ee40a0536baee3f539b019df5d.md) to delete The object. 


* [Luna::UniquePtr](class_luna_1_1_unique_ptr.md)

    A smart pointer that wraps one dynamically created object, and deletes the object when the pointer is destructed. 


* [Luna::Variant](class_luna_1_1_variant.md)

    Represents a dynamic typed object that stores data in a schema-less (self-described) manner. 


## Enumerations
* [Luna::SeekMode](group___runtime_1gaf2c27cfc991f5e917923e425d0bf1106.md)

    Specify the seek mode for one seekable stream. 

* [Luna::VariantType](group___runtime_1gac1ce0b9d7902d01bfd860c08aed25233.md)

    Defines all possible types of one [Variant](class_luna_1_1_variant.md) object. 

* [Luna::VariantNumberType](group___runtime_1ga736977eb95737aa8503b91d026bac3fa.md)

    Defines all possible number types of one number variant. 

## Functions
* [auto invoke(_Func &&f) -> decltype(static_cast< _Func && >(f)())](group___runtime_1gaf7411fc1e4c76b86c6f6b69eeb62b704.md)

    Invokes the specified callable object. 

* [auto invoke(_Func &&f, _Ty &&arg1, _Args &&... args) -> invoke_result_t< _Func, _Ty, _Args... >](group___runtime_1gaf7a93152ce0e85bc60d65da9d62c0ca7.md)

    Invokes the specified callable object. 

* [_Return invoke_r(_Func &&f, _Args &&... args)](group___runtime_1gac769aef9bea2b465a9437c25ac6ac9ac.md)

    Invokes the specified callable object. 

* [constexpr ReverseIterator< _Iter > make_reverse_iterator(_Iter i)](group___runtime_1gab53d4c159697d19e8fda0a022d611150.md)

    Creates one reverse iterator from one iterator. 

* [void advance(_Iter &it, _Distance n)](group___runtime_1gaeb004dafbae757b1fe66452065ae8739.md)

    Advances the given iterator by `n` positions respectively. 

* [isize distance(_It first, _It last)](group___runtime_1gacceb07c8bab688f75ae3207dea30f02e.md)

    Gets the number of elements between two iterators. 

* [_Iter next(_Iter it, isize n=1)](group___runtime_1ga4e2d965044b1d306278d256d980423fd.md)

    Gets one iterator to the next `n`th element of the element pointed by the input iterator. 

* [_BidirIt prev(_BidirIt it, isize n=1)](group___runtime_1ga3eab7cd933798dde3a66eb98069ea222.md)

    Gets one iterator to the last `n`th element of the element pointed by the input iterator. 

* [Ref< _Ty > box_ptr(_Ty *obj)](group___runtime_1ga9ffa672f4edd97e1402ea85d169de3aa.md)

    Creates a strong reference from one raw pointer without modifing its reference count. 

* [Ref< _Ty > new_object(_Args &&... args)](group___runtime_1gaa7e539a91bc5a8e68c91db8d2d8a9c23.md)

    Creates one new boxed object. 

* [TupleElement< _I, Tuple< _Tys... > >::type & get(Tuple< _Tys... > &t)](group___runtime_1ga9aae6d134b69bdfb7f054dcd50ddf57c.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type && get(Tuple< _Tys... > &&t)](group___runtime_1gacd20ef40077353ef2010188bf15f7efd.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type const  & get(const Tuple< _Tys... > &t)](group___runtime_1gaa2974b4a26c9dfcb6bb4d25d51be4a65.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type const  && get(const Tuple< _Tys... > &&t)](group___runtime_1gac24377ec6084290e12571664003bd153.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type volatile & get(volatile Tuple< _Tys... > &t)](group___runtime_1ga89f6c77e0282488319d7e9fcf5513350.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type volatile && get(volatile Tuple< _Tys... > &&t)](group___runtime_1gad849811e59b2a93e85659d4fe0bf7604.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type const volatile & get(const volatile Tuple< _Tys... > &t)](group___runtime_1ga6f00a23ba63eaefec5ff55bf6c8c269f.md)

    Gets the `_I`th element from the tuple. 

* [TupleElement< _I, Tuple< _Tys... > >::type const volatile && get(const volatile Tuple< _Tys... > &&t)](group___runtime_1ga573a4679d91cbf159ed82aaf27d2ce60.md)

    Gets the `_I`th element from the tuple. 

* [typeinfo_t tuple_type()](group___runtime_1gaf340d535f67d84438e25d13ef53faee8.md)

    Gets the type object of [Tuple](class_luna_1_1_tuple.md). 

