# Luna::JobSystem::is_job_finished

```c++
bool is_job_finished(job_id_t job)
```

Checks whether the specified job is finished. 



## Parameters
* *in* **job**

    The job ID to check. If this is [INVALID_JOB_ID](group___job_system_1gaa92b808b0484be3c6cfe8c792689cb18.md), this call always return `true`. 

## Return value
Returns `true` if the job is finished, `false` otherwise. 

