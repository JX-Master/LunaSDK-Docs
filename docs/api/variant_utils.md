# Variant Utils
[Variant](class_luna_1_1_variant.md) Utils module provides functions to operate [Luna::Variant](class_luna_1_1_variant.md) objects. 

## Functions
* [Variant diff(const Variant &before, const Variant &after)](group___variant_utils_1gad66978526bf62fd780e0696831c786e3.md)

    Creates one delta variant that stores changes from `before` to `after`. 

* [void patch(Variant &before, const Variant &delta)](group___variant_utils_1ga8e04de424e40ac3022ce8318acd4c297.md)

    Applys the difference to the variant, so that it contains the same data as `after` when the diff object is created. 

* [void revert(Variant &after, const Variant &delta)](group___variant_utils_1ga97c3d1b7451ad46f85d0359e5b055d65.md)

    Reverts the difference made in `after`, so that it contains the same data as `before` when the diff object is created. 

* [void add_diff_prefix(Variant &delta, Span< const Variant > prefix_nodes)](group___variant_utils_1ga359de28383997a81970af8ff2e57ef78.md)

    Adds prefix nodes to the delta object. 

* [R< Variant > read_json(const c8 *src, usize src_size=USIZE_MAX)](group___variant_utils_1ga752b6b9979f205bb3e0e1510d12441c3.md)

    Parses one JSON string. 

* [R< Variant > read_json(IStream *stream)](group___variant_utils_1ga68e89af46b6d1bc5c98f2474f809c148.md)

    Parses one JSON string. 

* [String write_json(const Variant &v, bool indent=true)](group___variant_utils_1ga6354edac5691a20766c78de8f1964745.md)

    Writes one variant object to JSON string. 

* [RV write_json(IStream *stream, const Variant &v, bool indent=true)](group___variant_utils_1ga875958329b5ebe521d30ad7dfbde82d6.md)

    Writes one variant object to JSON string. 

* [Variant new_xml_element(const Name &name)](group___variant_utils_1gad821aa5d9bc80323e60e4437f22be107.md)

    Creates one variant that represents one XML element. 

* [Name get_xml_name(const Variant &xml_element)](group___variant_utils_1ga66acb97e204dcc3c0c185570eb8f5920.md)

    Gets the name of one XML element. 

* [void set_xml_name(Variant &xml_element, const Name &name)](group___variant_utils_1ga0111e570290e610fdf21bb79ae74324d.md)

    Sets the name of one XML element. 

* [const Variant & get_xml_attributes(const Variant &xml_element)](group___variant_utils_1ga7b918421c87a4e944cc6fdc4e4bf0093.md)

    Gets attributes of one XML element. 

* [Variant & get_xml_attributes(Variant &xml_element)](group___variant_utils_1gacd1a3a6473c2c903b021ebf25a56665c.md)

    Gets attributes of one XML element. 

* [const Variant & get_xml_content(const Variant &xml_element)](group___variant_utils_1gae5d5f3e6c96251cf9be0ee0d0324f76c.md)

    Gets content of one XML element. 

* [Variant & get_xml_content(Variant &xml_element)](group___variant_utils_1gac504b357b0818e0958861de2ddf994b8.md)

    Gets content of one XML element. 

* [const Variant & find_first_xml_child_element(const Variant &xml_element, const Name &name, usize start_index=0, usize *out_index=nullptr)](group___variant_utils_1ga29f95d2c8b503535511b7c79f264c018.md)

    Finds the first XML child element in the specified XML element with the specified name. 

* [R< Variant > read_xml(const void *src, usize src_size=USIZE_MAX)](group___variant_utils_1ga7fff1e398a7f8a0d35da1ef427a84716.md)

    Parses one XML string. 

* [R< Variant > read_xml(IStream *stream)](group___variant_utils_1ga43fd40bab1388020d111162dc9d28b8b.md)

    Parses one XML string. 

* [String write_xml(const Variant &v, bool indent=true)](group___variant_utils_1ga97d3e633d9eb6f12ab085f8a4069a613.md)

    Writes one variant object to XML string. 

* [RV write_xml(IStream *stream, const Variant &v, bool indent=true)](group___variant_utils_1ga3d795b79b237a7986984f91e03d210f3.md)

    Writes one variant object to XML string. 

