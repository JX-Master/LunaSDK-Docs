# Luna::Event::operator()

```c++
template <typename...>
void operator()(_Args &&... args)
```

Triggers this event and invokes all handlers. 



## Parameters
* *in* **args**

    [Event](class_luna_1_1_event.md) arguments that will be broadcasted to every handler of this event. 

