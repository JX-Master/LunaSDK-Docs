# Luna::VariantUtils::add_diff_prefix

```c++
void add_diff_prefix(Variant &delta, Span< const Variant > prefix_nodes)
```

Adds prefix nodes to the delta object. 

This can be used if the delta object is computed from a child variant, but the user wants to patch the delta object to a parent variant. See remarks for details. 

## Parameters
* *in* **delta**

    The delta object to modify. 

* *in* **prefix_nodes**

    The prefix nodes to add to the delta object. 

## Remark
For example, if we have the following variant: 
```
{
    "rootRegion":
    {
        "members":
        [
            {
                "row":2
            }
        ]
    }
}
```
 and we have the following delta: 
```
{
    "row": [2,3]
}
```
 after adding prefix nodes `{ "rootRegion", "members", (u64)0 }` to the delta, the result delta object will be: 
```
{
    "rootRegion": {
        "members": {
            "_t": "a",
            "0": {
                "row": [2,3]
            }
        }
    }
}
```
 which can be used to change the value of ["rootRegion"]["members"][0]["rows"] from 2 to 3. 

