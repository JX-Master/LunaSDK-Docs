# Luna::ECS::ITaskContext::begin

```c++
virtual void begin(IWorld *world, TaskExecutionMode exec_mode, Span< typeinfo_t > read_components, Span< typeinfo_t > write_components)=0
```

Resets the task context and begins a new task. 



## Parameters
* *in* **world**

    The world to run the task on. 

* *in* **exec_mode**

    The task execution mode. 

* *in* **read_components**

    When `exec_mode` is `shared`, specify components that will be read from by this task. 

* *in* **write_components**

    When `exec_mode` is `shared`, specify components that will be read from and written to by this task. 

## Remark
This call may block the current thread until all components required by this task can be safely accessed by this task, or until all other tasks are finished if this is a exclusive task. 

