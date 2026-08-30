# Azure Terraform — Resource Group Demo

DevOps coursework project that uses Terraform to provision a resource group on Microsoft Azure.

## 📁 Project Structure

```
azure-Aug-/
├── main.tf              # Defines the azurerm_resource_group resource
├── providers.tf          # Azure provider configuration
├── variables.tf          # Input variable declarations
├── outputs.tf            # Output values after apply
├── .terraform.lock.hcl    # Provider version lock file
└── .gitignore             # Ignores .terraform/ and state files
```

## 🚀 What it does

Running this configuration creates a single Azure Resource Group:

| Resource | Name | Location |
|---|---|---|
| `azurerm_resource_group` | `TerraformDemoRG` | Central India |

## 🛠️ Prerequisites

- [Terraform](https://developer.hashicorp.com/terraform/downloads) installed (v1.x)
- An active [Azure account](https://azure.microsoft.com/)
- [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli) installed and authenticated:
  ```bash
  az login
  ```

## ▶️ Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/itzsonu/azure-Aug-.git
   cd azure-Aug-
   ```

2. **Initialize Terraform**
   ```bash
   terraform init
   ```

3. **Preview the changes**
   ```bash
   terraform plan
   ```

4. **Apply the configuration**
   ```bash
   terraform apply
   ```

5. **Destroy resources** (to avoid unnecessary Azure charges once done)
   ```bash
   terraform destroy
   ```

## 📌 Notes

- `.terraform/` and `*.tfstate*` files are excluded from version control via `.gitignore`, since they may contain sensitive data.
- This project is for academic/learning purposes as part of DevOps coursework.
