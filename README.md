# Terraform Learning with Azure

A day-by-day collection of Terraform exercises for learning how to provision and manage Microsoft Azure infrastructure. Each day focuses on one Terraform concept and keeps the example code in its own folder.

## Learning path

The folder names below are the friendly names used for this learning path. A `Planned` entry describes the next folder to be added; only completed folders are linked to avoid broken GitHub navigation.

| Day | Topic | Folder | Status |
| --- | --- | --- | --- |
| 1 | Terraform provider and Azure resource |`01-provider-and-azure-resources` | Complete |
| 2 | Create an Azure Storage Account | `02-azure-storage-account` | Planned |
| 3 | Manage Terraform state with Azure Storage | `03-remote-state-with-azure-storage` | Planned |
| 4 | Input, output, and local variables | `04-terraform-variables` | Planned |
| 5 | Terraform file and directory structure | `05-project-structure-best-practices` | Planned |
| 6 | Terraform type constraints | `06-type-constraints` | Planned |
| 7 | Resource meta-arguments: `count` and `for_each` | `07-count-and-for-each` | Planned |
| 8 | Lifecycle rules: create before destroy, prevent destroy, and ignore changes | `08-resource-lifecycle-rules` | Planned |
| 9 | Dynamic, conditional, and splat expressions | `09-terraform-expressions` | Planned |
| 10 | Terraform functions | `10-terraform-functions` | Planned |
| 11 | Terraform functions, part 2 | `11-terraform-functions-part-2` | Planned |
| 12 | Azure data sources | `12-azure-data-sources` | Planned |
| 13 | Production-grade Azure infrastructure and auto-scaling | `13-production-azure-infrastructure` | Planned |
| 14 | Azure virtual network peering | `14-azure-vnet-peering` | Planned |
| 15 | Azure Entra ID and identity management | `15-azure-entra-id` | Planned |
| 16 | Azure App Service and blue-green deployment | `16-azure-app-service-blue-green` | Planned |
| 17 | Azure Functions QR code generator | `17-azure-functions-qr-code-generator` | Planned |

## Getting started

### Prerequisites

- [Terraform](https://developer.hashicorp.com/terraform/install) installed locally
- An Azure subscription
- [Azure CLI](https://learn.microsoft.com/cli/azure/install-azure-cli) installed and authenticated

Sign in to Azure before running an exercise:

```bash
az login
```

### Run an exercise

From the exercise folder, initialize Terraform, review the planned changes, and apply them when ready:

```bash
terraform init
terraform fmt
terraform validate
terraform plan
terraform apply
```

When you finish, remove resources that are no longer needed:

```bash
terraform destroy
```

## Repository conventions

- Each day has an isolated Terraform configuration.
- Azure provider versions are pinned in `required_providers` when the exercise needs a provider.
- Resource names and values are intentionally simple so the Terraform concepts remain easy to follow.
- Never commit secrets, service principal credentials, or Terraform state files containing sensitive values.

## Progress

- [x] Day 1: Provider and Azure resources
- [ ] Days 2-17: Upcoming exercises