# Luna::RHI::IQueryHeap::get_timestamp_values

```c++
virtual RV get_timestamp_values(u32 index, u32 count, u64 *values)=0
```

Copies timestamp query results from query heap to the user-provided buffer. 



## Parameters
* *in* **index**

    The index of the first query to copy. 

* *in* **count**

    The number of queries to copy. 

* *out* **values**

    The user-provided buffer used to store the results. 

## Remark
The user must ensure that all queries being copied are initialized, or the behavior is undefined. If this query heap is not `QueryHeapType::timestamp`, this function fails with `BasicError::not_supported`. 

