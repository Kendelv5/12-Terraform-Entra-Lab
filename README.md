Lab 12: Terraform Azure Entra ID Provisioning

Overview
This lab demonstrates how to use Terraform with the HashiCorp AzureAD provider to automate identity and access management tasks inside Microsoft Entra ID.

Objectives

Configure an Azure App Registration with appropriate Microsoft Graph API permissions for Infrastructure as Code.

Declare and provision an Entra ID security group.

Provision a test user account within the tenant's verified domain.

Establish a group membership relationship using raw object ID references.

Architecture and Resources

Provider: hashicorp/azuread

Resources:

azuread_group (terraform_sec_group)

azuread_user (terraform_test_user)

azuread_group_member (membership)

Execution Steps

Initialize the provider plugins:
terraform init

Execute the infrastructure deployment plan:
terraform apply
