# Luna::JobSystem::submit_job

```c++
job_id_t submit_job(void *params)
```

Submits the job to the job system. 



## Parameters
* *in* **params**

    The parameter block pointer of the job. Every job can only be submitted once. If the parameter block is not trivially destructable, the user must destruct the parameter block manually at the end of the job callback function. 

## Return value
Returns the job ID for the submitted job, which can be used to wait for the job using [wait_job](group___job_system_1gaa3022beece29b6efd1d4f00d9cc6f522.md), or check whether the job is finished using [is_job_finished](group___job_system_1ga1eca8cb83f5a85979d52b5431628e8b9.md). 

