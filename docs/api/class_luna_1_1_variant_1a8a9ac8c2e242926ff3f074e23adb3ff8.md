# Luna::Variant::find_or_insert

```c++
Variant & find_or_insert(const Name &k)
```

Gets the child variant with the specified key, or inserts one new child variant with that key if not exists. 



## Parameters
* *in* **k**

    The key string of the child variant to fetch or insert. 

## Return value
Returns one reference to the found or inserted child variant. 

## Remark
The variant inserted by this function will have [VariantType::null](group___runtime_1ggac1ce0b9d7902d01bfd860c08aed25233a37a6259cc0c1dae299a7866489dff0bd.md) type. 

## Valid Usage
* The current variant must be an object variant or a null variant. If the variant is a null variant, it will be transformed into one object variant before the new key-variant pair is inserted. 

