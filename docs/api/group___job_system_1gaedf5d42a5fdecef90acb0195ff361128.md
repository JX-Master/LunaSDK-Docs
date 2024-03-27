# Luna::JobSystem::new_job

```c++
void * new_job(job_func_t *func, usize param_size, usize param_alignment, void *parent=nullptr)
```

Creates a new job. 



## Parameters
* *in* **func**

    The job callback function to invoke. 

* *in* **param_size**

    The size of the parameter block. 

* *in* **param_alignment**

    The alignment of the parameter block. 

* *in* **parent**

    The optional parameter pointer of the parent job. If this is not `nullptr`, all waits for the parent job will wait this job as well. 

## Return value
Returns the parameter block pointer of the created job. The parameter block data is uninitialized and should be initialized by the user. 

