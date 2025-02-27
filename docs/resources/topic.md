---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "pulsar_topic Resource - terraform-provider-pulsar"
subcategory: ""
description: |-
  
---

# pulsar_topic (Resource)





<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `namespace` (String) Pulsar namespaces are logical groupings of topics
- `partitions` (Number)
- `tenant` (String) An administrative unit for allocating capacity and enforcing an 
authentication/authorization scheme
- `topic_name` (String)
- `topic_type` (String)

### Optional

- `permission_grant` (Block Set) (see [below for nested schema](#nestedblock--permission_grant))
- `retention_policies` (Block Set, Max: 1) (see [below for nested schema](#nestedblock--retention_policies))

### Read-Only

- `id` (String) The ID of this resource.

<a id="nestedblock--permission_grant"></a>
### Nested Schema for `permission_grant`

Required:

- `actions` (Set of String)
- `role` (String)


<a id="nestedblock--retention_policies"></a>
### Nested Schema for `retention_policies`

Required:

- `retention_size_mb` (Number)
- `retention_time_minutes` (Number)


