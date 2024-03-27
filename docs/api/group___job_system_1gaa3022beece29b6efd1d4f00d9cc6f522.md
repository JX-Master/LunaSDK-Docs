# Luna::JobSystem::wait_job

```c++
void wait_job(job_id_t job)
```

Blocks the current thread to wait for the job to finish. 



## Parameters
* *in* **job**

    The job ID to wait. If this is [INVALID_JOB_ID](group___job_system_1gaa92b808b0484be3c6cfe8c792689cb18.md), this call returns immediately. 

