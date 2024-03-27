# Luna::JobSystem::get_current_job_id

```c++
job_id_t get_current_job_id(void *params)
```

Fetches the job ID assigned with the specified job. 



## Parameters
* *in* **params**

    The parameter block pointer of the job. 

## Return value
Returns the assigned job ID for the job. Returns [INVALID_JOB_ID](group___job_system_1gaa92b808b0484be3c6cfe8c792689cb18.md) if the job is not submitted yet. 

