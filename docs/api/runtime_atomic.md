# Atomic Operations
## Functions
* [i32 atom_inc_i32(i32 volatile *v)](group___runtime_atomic_1ga93fd78ec313117f79a24d3417839a990.md)

    Atomically increase the value of the variable by 1. 

* [u32 atom_inc_u32(u32 volatile *v)](group___runtime_atomic_1ga6518f9b14abc2ee70d4091514214dfbf.md)

    Atomically increase the value of the variable by 1. 

* [i64 atom_inc_i64(i64 volatile *v)](group___runtime_atomic_1gae708cad0929be90c9168ba2928578b47.md)

    Atomically increase the value of the variable by 1. 

* [u64 atom_inc_u64(u64 volatile *v)](group___runtime_atomic_1gaa488e7d5ebb05db6c71c3ec64448d4df.md)

    Atomically increase the value of the variable by 1. 

* [usize atom_inc_usize(usize volatile *v)](group___runtime_atomic_1ga69573d3b1723490896654b184576459f.md)

    Atomically increase the value of the variable by 1. 

* [i32 atom_dec_i32(i32 volatile *v)](group___runtime_atomic_1gadf6d183e6f826c4d6a090edec5a8fdda.md)

    Atomically decrease the value of the variable by 1. 

* [u32 atom_dec_u32(u32 volatile *v)](group___runtime_atomic_1ga5d80a9933e7c6fd8b1aeffae59a9401e.md)

    Atomically decrease the value of the variable by 1. 

* [i64 atom_dec_i64(i64 volatile *v)](group___runtime_atomic_1ga2edbadd594f46bf5a723bbb862816a7e.md)

    Atomically decrease the value of the variable by 1. 

* [u64 atom_dec_u64(u64 volatile *v)](group___runtime_atomic_1ga9eab0a468ed18345fd61ca078ff0ad2d.md)

    Atomically decrease the value of the variable by 1. 

* [usize atom_dec_usize(usize volatile *v)](group___runtime_atomic_1gad1ea6147a2eb3dcacaa983ff8ed4ceed.md)

    Atomically decrease the value of the variable by 1. 

* [i32 atom_add_i32(i32 volatile *base, i32 v)](group___runtime_atomic_1ga87e1475faf37125af9943c8b57477523.md)

    Atomically increase the value of the variable by the the value provided. 

* [u32 atom_add_u32(u32 volatile *base, i32 v)](group___runtime_atomic_1ga49d341d1f579fbab68f5ef1132bd473c.md)

    Atomically increase the value of the variable by the the value provided. 

* [i64 atom_add_i64(i64 volatile *base, i64 v)](group___runtime_atomic_1gab6bd5e2b180aad4f2d558a34140bc995.md)

    Atomically increase the value of the variable by the the value provided. 

* [u64 atom_add_u64(u64 volatile *base, i64 v)](group___runtime_atomic_1ga8983ea053ce60d5d84ab0bed9b62a4fb.md)

    Atomically increase the value of the variable by the the value provided. 

* [usize atom_add_usize(usize volatile *base, isize v)](group___runtime_atomic_1gaded38c04fc62137615098589f994570c.md)

    Atomically increase the value of the variable by the the value provided. 

* [i32 atom_exchange_i32(i32 volatile *dst, i32 v)](group___runtime_atomic_1ga4dfa84dda4fc0790182c43da18d9b7ba.md)

    Atomically replace the value of the variable with the value provided. 

* [u32 atom_exchange_u32(u32 volatile *dst, u32 v)](group___runtime_atomic_1gaecf689ac29ab761332abbdb15ce2b7a2.md)

    Atomically replace the value of the variable with the value provided. 

* [i64 atom_exchange_i64(i64 volatile *dst, i64 v)](group___runtime_atomic_1ga1d9de4afb248d2c77378e1ea7b7a36cd.md)

    Atomically replace the value of the variable with the value provided. 

* [u64 atom_exchange_u64(u64 volatile *dst, u64 v)](group___runtime_atomic_1ga968dc37e8476a93bda283261d818af2a.md)

    Atomically replace the value of the variable with the value provided. 

* [_Ty * atom_exchange_pointer(_Ty *volatile *target, void *value)](group___runtime_atomic_1gad90ccf004b120e9777e9d57f55315887.md)

    Atomically replace the value of the variable with the value provided. 

* [usize atom_exchange_usize(usize volatile *dst, usize v)](group___runtime_atomic_1ga7863b3a44ba17280c9e03b50d4e7f70e.md)

    Atomically replace the value of the variable with the value provided. 

* [i32 atom_compare_exchange_i32(i32 volatile *dst, i32 exchange, i32 comperand)](group___runtime_atomic_1gaf678d9768b4d454a41fccf2b33eb1f2a.md)

    Atomically compares the value of the variable with the specified comperand, and sets the variable to the specified value if equal. 

* [u32 atom_compare_exchange_u32(u32 volatile *dst, u32 exchange, u32 comperand)](group___runtime_atomic_1ga052ebc68d59e6cd7e925a6fba665d837.md)

    Atomically compares the value of the variable with the specified comperand, and sets the variable to the specified value if equal. 

* [_Ty * atom_compare_exchange_pointer(_Ty *volatile *dst, void *exchange, void *comperand)](group___runtime_atomic_1ga81153c02015584994d148c7b52c16ceb.md)

    Atomically compares the value of the variable with the specified comperand, and sets the variable to the specified value if equal. 

* [usize atom_compare_exchange_usize(usize volatile *dst, usize exchange, usize comperand)](group___runtime_atomic_1gad23be0a05e525acf2b27afc09d89c2ed.md)

    Atomically compares the value of the variable with the specified comperand, and sets the variable to the specified value if equal. 

