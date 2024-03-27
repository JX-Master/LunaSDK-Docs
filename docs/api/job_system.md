# Job System
Job system module provides thread pool to execute jobs asynchronously for a multithreaded computer program. 

## Alias types
* [using job_id_t =  u64](group___job_system_1gad8224d6227de57a1a88f36a526447549.md)

    Identifies one job that can be waited. 

* [using job_func_t =  void(void* params)](group___job_system_1ga741d15f2a9c0d352bbc48af082e349f5.md)

    The callback function of one job. 

## Constants
* [constexpr job_id_t INVALID_JOB_ID](group___job_system_1gaa92b808b0484be3c6cfe8c792689cb18.md)

    A special ID that identifies one invalid job. 

## Functions
* [job_id_t allocate_job_id()](group___job_system_1ga832ccddd2391a3edf9663e14e138b105.md)

    Allocates one job ID, so that other threads can wait for it by calling [wait_job](group___job_system_1gaa3022beece29b6efd1d4f00d9cc6f522.md). 

* [void finish_job_id(job_id_t job)](group___job_system_1gae4cf2717534772d29563d86e2c53257a.md)

    Marks one job ID as finished, so that all jobs waiting for this job ID will be resumed. This function should only be called for job IDs allocated by [allocate_job_id](group___job_system_1ga832ccddd2391a3edf9663e14e138b105.md), never call this function for job IDs returned by [submit_job](group___job_system_1gabcf07bd4ba10790a7426b555ab541c17.md). See remarks of [allocate_job_id](group___job_system_1ga832ccddd2391a3edf9663e14e138b105.md) for details. 

* [void * new_job(job_func_t *func, usize param_size, usize param_alignment, void *parent=nullptr)](group___job_system_1gaedf5d42a5fdecef90acb0195ff361128.md)

    Creates a new job. 

* [job_id_t submit_job(void *params)](group___job_system_1gabcf07bd4ba10790a7426b555ab541c17.md)

    Submits the job to the job system. 

* [job_id_t get_current_job_id(void *params)](group___job_system_1ga56f8bc22701bd6f691983bdadf5e6351.md)

    Fetches the job ID assigned with the specified job. 

* [void wait_job(job_id_t job)](group___job_system_1gaa3022beece29b6efd1d4f00d9cc6f522.md)

    Blocks the current thread to wait for the job to finish. 

* [bool is_job_finished(job_id_t job)](group___job_system_1ga1eca8cb83f5a85979d52b5431628e8b9.md)

    Checks whether the specified job is finished. 

