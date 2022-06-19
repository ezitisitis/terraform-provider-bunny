---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "bunny_hostname Resource - bunny"
subcategory: ""
description: |-
  
---

# bunny_hostname (Resource)





<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `hostname` (String) The hostname value for the domain name.
- `pull_zone_id` (Number) The ID of the pull zone to that the hostname belongs.

### Optional

- `certificate` (Block List, Max: 1) Specifies a custom SSL certificate for the hostname. (see [below for nested schema](#nestedblock--certificate))
- `force_ssl` (Boolean) Determines if the Force SSL feature is enabled.
- `load_free_certificate` (Boolean) Determines if a free SSL certificate should be generated and loaded for the hostname

### Read-Only

- `has_certificate` (Boolean) Determines if the hostname has an SSL certificate configured.
- `id` (String) The ID of this resource.
- `is_system_hostname` (Boolean) Determines if this is a system hostname controlled by bunny.net.

<a id="nestedblock--certificate"></a>
### Nested Schema for `certificate`

Required:

- `certificate_data` (String) The X.509 certificate.
- `private_key_data` (String, Sensitive) The private key.

