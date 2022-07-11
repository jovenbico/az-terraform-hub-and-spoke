# AZ Terraform Hub and Spoke

## Prerequisite
1. Terraform
```
$ terraform version

Terraform v1.2.4
on linux_amd64
+ provider registry.terraform.io/hashicorp/azurerm v2.99.0
```
2. Azure cli
```
$ az version
{
  "azure-cli": "2.38.0",
  "azure-cli-core": "2.38.0",
  "azure-cli-telemetry": "1.0.6",
  "extensions": {}
}
```

3. Create Azure cloud sanbox
```
## Update resource group (rg-name) local variable

locals {
  rg-name        = "1-xyz-playground-sandbox"
}
```

## Initialize terraform code
```
$ terraform init
$ terraform fmt
$ terraform plan
```

## Deploy terraform code
```
$ terraform apply --auto-approve
```