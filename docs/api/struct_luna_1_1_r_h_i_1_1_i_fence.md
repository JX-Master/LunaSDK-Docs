# Luna::RHI::IFence
Represents a synchronization object that can be used to synchronize commands executed in different command queues. 

```c++
interface Luna::RHI::IFence : public virtual IDeviceChild
```

A fence is a synchronization primitive that can be used to insert a dependency between queue operations. When the user submits one queue operation, she may specify multiple fences as either wait targets or signal targets. Before the device processes the operation, it will firstly waits for all wait targets to be signaled. After the device processes the operation, it will signal all signal targets, so that other operations waiting on these fences can be processed.

Every fence has two states: signaled and unsignaled. The fence state is managed by the device automatically, one fence is created in unsignaled state, every signal operation changes the fence state from unsignaled to signaled, and every wait operation resets the fence state to unsignaled. To use fence objects properly, the user must ensure that signal operations and wait operations on the same fence should occur in discrete 1:1 pairs (every two signal operations should have one wait operations in between, every two wait operations should one signal operations in between). 

## Base type
* [IDeviceChild](struct_luna_1_1_r_h_i_1_1_i_device_child.md)
