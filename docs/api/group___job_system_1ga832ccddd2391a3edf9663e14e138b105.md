# Luna::JobSystem::allocate_job_id

```c++
job_id_t allocate_job_id()
```

Allocates one job ID, so that other threads can wait for it by calling [wait_job](group___job_system_1gaa3022beece29b6efd1d4f00d9cc6f522.md). 



## Return value
Returns the allocated job ID. 

## Remark
This function is called internally by the job system for all jobs submitted by [submit_job](group___job_system_1gabcf07bd4ba10790a7426b555ab541c17.md), so the user doesn't need to call this function manually. However, the job ID can also be used solely without submitting any job to provide a synchronizing point that other threads can wait for.


Every allocated job ID must be finished by calling [finish_job_id](group___job_system_1gae4cf2717534772d29563d86e2c53257a.md), or memory leak will occur. For job IDs created by [submit_job](group___job_system_1gabcf07bd4ba10790a7426b555ab541c17.md), the job system calls [finish_job_id](group___job_system_1gae4cf2717534772d29563d86e2c53257a.md) automatically when the job callback function returns, so the user should not finish it manually. But for job IDs created by [allocate_job_id](group___job_system_1ga832ccddd2391a3edf9663e14e138b105.md), the user should call [finish_job_id](group___job_system_1gae4cf2717534772d29563d86e2c53257a.md) manually to correctly finish them. 

