# Simple shared VPC Project

This example:

* Enables shared VPC on a host project
* Attaches a service project
* Reserves an internal IP address in a subnet of a Shared VPC network

Note that the IP address configuration object is created in the service
project, while its value comes from the range of available addresses in
the chosen shared subnet.


<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| project | The host project ID | `any` | n/a | yes |
| service\_project | The service project ID | `any` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| ip\_address | The internal IP address |
| ip\_address\_name | The name of the internal IP |
| project | Host project ID |
| subnet | Name of the host subnet |

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
