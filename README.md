# Lab 12: Azure Entra ID Resource Provisioning with Terraform

## Overview
Automating identity and access management operations inside Microsoft Entra ID utilizing Terraform and the HashiCorp AzureAD provider.

## Objectives
- Authenticate Terraform against Azure AD using an App Registration and Service Principal.
- Provision an Entra ID security group with descriptive attributes.
- Provision a test user account mapped to the tenant's verified domain name.
- Establish a dynamic group membership link utilizing raw object IDs.

## Lab Architecture & Resources
- **`versions.tf`**: Configures the required AzureAD provider version and authentication variables (`client_id`, `client_secret`, `tenant_id`).
- **`main.tf`**: Declares the target resources (`azuread_group`, `azuread_user`, and `azuread_group_member`).

## Step-by-Step Implementation

### Step 1: Initialize Working Directory
Run initialization to download the HashiCorp AzureAD provider plugins:

### Step 2: Execute Deployment Plan
Review the infrastructure changes and apply the configuration to build your resources:

### Step 3: Verification
Navigate to the **Microsoft Entra ID** portal dashboard to confirm your security group and test user are successfully provisioned and mapped.
