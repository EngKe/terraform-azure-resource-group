# Azure Resource Group Terraform Module

This Terraform module creates an Azure Resource Group.

## Usage

```hcl
module "resource_group" {
  source              = "git::https://github.com/yourusername/yourrepository.git//path-to-module"
  resource_group_name = "example-rg"
  location            = "West Europe"
}
```

### Inputs

| Name                  | Description                             | Type   | Default     | Required |
|-----------------------|-----------------------------------------|--------|-------------|----------|
| `resource_group_name` | The name of the resource group          | string | n/a         | yes      |
| `location`            | The location of the resource group      | string | `"East US"` | no       |

## Outputs

| Name                  | Description                             |
|-----------------------|-----------------------------------------|
| `resource_group_name` | The name of the resource group          |


### Requirements

| Name       | Version |
|------------|---------|
| `terraform` | >= 0.12 |
| `azurerm`   | >= 2.0  |

## Providers

| Name      | Version |
|-----------|---------|
| `azurerm` | >= 2.0  |

## Resources

| Name                             | Type     |
|----------------------------------|----------|
| `azurerm_resource_group.example` | resource |

## Author

This module is maintained by [Your Name](https://github.com/yourusername).

## License

This module is licensed under the MIT License. See the LICENSE file for details.
