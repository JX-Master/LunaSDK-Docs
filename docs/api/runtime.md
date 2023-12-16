# Runtime
Represents a waitable object used for multi-thread synchronization. 

The Runtime module provides the runtime environment of Luna SDK and defines core functionalities that will be used by almost all modules.

Objects that implements `IWaitable` cannot be used cross process boundary. 

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
* [Memory allocation and deallocation](runtime_memory.md)
* [Memory utility library](runtime_memory_utils.md)
* [Module system](runtime_module.md)
* [Name strings](runtime_name.md)
* [Boxed objects](runtime_object.md)
* [Path](runtime_path.md)
* [Debugging](runtime_profiler.md)
* [Generating random numbers](runtime_random.md)
* [SDK initialization and shutdown](runtime_init.md)
* [Thread management and synchronization methods](runtime_thread.md)
* [Type reflection](runtime_type.md)
* [Unicode encoding/decoding](runtime_unicode.md)
## Classes
* [Luna::Allocator](class_luna_1_1_allocator.md)
* [Luna::Blob](class_luna_1_1_blob.md)
* [Luna::Event](class_luna_1_1_event.md)
* [Luna::equal_to](struct_luna_1_1equal__to.md)
* [Luna::less](struct_luna_1_1less.md)
* [Luna::hash](struct_luna_1_1hash.md)
* [Luna::ReferenceWrapper](class_luna_1_1_reference_wrapper.md)
* [Luna::Function< _R(_Args...)>](struct_luna_1_1_function_3_01___r_07___args_8_8_8_08_4.md)
* [Luna::ReverseIterator](class_luna_1_1_reverse_iterator.md)
* [Luna::ObjRef](class_luna_1_1_obj_ref.md)
* [Luna::Ref](class_luna_1_1_ref.md)
* [Luna::WeakObjRef](class_luna_1_1_weak_obj_ref.md)
* [Luna::WeakRef](class_luna_1_1_weak_ref.md)
* [Luna::IStream](struct_luna_1_1_i_stream.md)
* [Luna::ISeekableStream](struct_luna_1_1_i_seekable_stream.md)
* [Luna::Variant](class_luna_1_1_variant.md)
* [Luna::Vector](class_luna_1_1_vector.md)
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

    Gets one iterator pointing to the next `n`th element of the element pointed by the input iterator. 

* [_BidirIt prev(_BidirIt it, isize n=1)](group___runtime_1ga3eab7cd933798dde3a66eb98069ea222.md)

    Gets one iterator pointing to the last `n`th element of the element pointed by the input iterator. 

* [Ref< _Ty > box_ptr(_Ty *obj)](group___runtime_1ga9ffa672f4edd97e1402ea85d169de3aa.md)

    Creates a strong reference from one raw pointer without modifing its reference count. 

* [Ref< _Ty > new_object(_Args &&... args)](group___runtime_1gaa7e539a91bc5a8e68c91db8d2d8a9c23.md)

    Creates one new boxed object. 

