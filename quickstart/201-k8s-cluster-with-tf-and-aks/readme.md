# Kubernetes cluster with Azure Kubernetes Service (AKS)

This template provisions an [AKS / Azure Kubernetes service (also known as a Managed Kubernetes Cluster)](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/kubernetes_cluster).

- [random_string](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/string)

## Terraform resource types

- [random_pet](https://registry.terraform.io/providers/hashicorp/random/latest/docs/resources/pet)
- [azurerm_resource_group](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/resource_group)
- [azurerm_client_config](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/data-sources/client_config)
- [azurerm_log_analytics_workspace](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/log_analytics_workspace)
- [azurerm_log_analytics_solution](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/log_analytics_solution)
- [azurerm_kubernetes_cluster](https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/kubernetes_cluster)
- [azuread_application](https://registry.terraform.io/providers/hashicorp/azuread/latest/docs/data-sources/application)
- [azuread_service_principal](https://registry.terraform.io/providers/hashicorp/azuread/latest/docs/data-sources/service_principal)
- [azuread_service_principal_password](https://registry.terraform.io/providers/hashicorp/azuread/latest/docs/resources/service_principal_password)
- [azapi_resource](https://registry.terraform.io/providers/Azure/azapi/latest/docs/resources/azapi_resource)
- [azapi_resource_action](https://registry.terraform.io/providers/Azure/azapi/latest/docs/resources/azapi_resource_action)

## Variables

| Name | Description | Default |
|-|-|-|
| `resource_group_name_prefix` | Prefix of the resource group name that's combined with a random ID so name is unique in your Azure subscription. | rg |
| `resource_group_location` | Location of the resource group. | eastus |
| `node_count` | Initial number of nodes which should exist in this Node Pool. Value must be between 1 and 1000. | 3 |
| `log_analytics_workspace_location` | Location of the Log Analytics workspace. | eastus |
| `log_analytics_workspace_sku` | SKU of the Log Analytics workspace. The SKU of the log analytics workspace. Choose from: Free, PerNode, Premium, Standard, Standalone, Unlimited, CapacityReservation, PerGB2018 | PerGB2018 |

## Example

To see how to run this example, see [Create a Kubernetes cluster with Azure Kubernetes Service using Terraform](https://docs.microsoft.com/azure/developer/terraform/create-k8s-cluster-with-tf-and-aks).
