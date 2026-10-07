# Azure Terraform Infrastructure

This repository contains Terraform configuration for provisioning Azure resources.

## Overview

The project is intended to manage infrastructure as code using Terraform and Azure Resource Manager.

## Prerequisites

Before running this project, make sure you have:

- [Terraform](https://developer.hashicorp.com/terraform/install)
- [Azure CLI](https://learn.microsoft.com/cli/azure/install-azure-cli)
- An Azure subscription
- Access to a valid Azure tenant

## Azure login

```bash
az login
az account set --subscription "<your-subscription-id-or-name>"
```

## Initialize Terraform

```bash
terraform init
```

## Validate the configuration

```bash
terraform validate
```

## Preview changes

```bash
terraform plan
```

## Apply the infrastructure

```bash
terraform apply
```

## Destroy the infrastructure

```bash
terraform destroy
```

## Project structure

```text
.
├── main.tf
├── provider.tf
├── terraform.tfstate
├── terraform.tfstate.backup
├── README.md
└── .gitignore
```

## Notes

- Review and update resource names, locations, and variables before deploying to production.
- Do not commit sensitive values or credentials.
- Use environment variables or secure secret management where appropriate.

## License

This project is provided for infrastructure automation purposes.
