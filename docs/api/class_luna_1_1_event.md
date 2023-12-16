# Luna::Event
Represents one event that once triggered, invokes all handlers registered to it. 

```c++
class Luna::Event
```

## Member functions
* [void clear()](class_luna_1_1_event_1ac8bb3912a3ce86b15842e79d0b421204.md)

    Removes all handlers registered to this event. 

* [void operator()(_Args &&... args)](class_luna_1_1_event_1ade9efb83ab8d8b52bd615583ffa59154.md)

    Triggers this event and invokes all handlers. 

* [usize add_handler(const Function< _Func > &func)](class_luna_1_1_event_1a161bc3ee47a2cafb32e491f5e5173095.md)

    Adds one new handler to the event. 

* [usize add_handler(Function< _Func > &&func)](class_luna_1_1_event_1a1dd8c836acc6e725ac36bbc658531913.md)

    Adds one new handler to the event. 

* [void remove_handler(usize handle)](class_luna_1_1_event_1a574c6b9a7157bcd241142910d6476f9e.md)

    Removes one registered handler. 

