---
categories: Azure
tags: ['Terraform', 'DevOps', 'InfrastructureAsCode', 'GitOps', 'Kubernetes']
is_post: "True"
is_home_btn_reqd: "True"
---

# Terraform Cheat Sheet
## Terraform CLI tricks
`terraform -install-autocomplete` #Setup tab auto-completion, requires logging back in

### Format and Validate Terraform code
`terraform fmt` # format code per HCL canonical standard

`terraform validate` #validate code for syntax

`terraform validate -backend=false` #validate code skip backend validation

### Initialize your Terraform working directory
`terraform init` #initialize directory, pull down providers

`terraform init -get-plugins=false` #initialize directory, do not download plugins

`terraform init -verify-plugins=false` #initialize directory, do not verify plugins for Hashicorp signature
