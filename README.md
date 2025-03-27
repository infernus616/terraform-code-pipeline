# AWS Organization Setup Guide

## Overview

This repository provides the necessary configuration files to set up the following AWS infrastructure:

- **AWS Organization** with the following three accounts:
  - `users`
  - `staging`
  - `production`
- **IAM Groups and Roles** for developer access.
- **Terraform Backend** configuration using an S3 bucket and DynamoDB table.

---

## Quickstart Guide

To get started, follow these steps:

1. **Update Configuration:**
   - Replace placeholder values in the [locals.tf](locals.tf) file with actual values based on your setup.

2. **Optional - Add Users:**  
   - To include users, edit the [users.tf](users.tf) file as needed.
   - For detailed instructions, refer to [adding-a-user.md](docs/adding-a-user.md).

3. **Initialize Terraform and Apply the Plan:**  
   Run the following commands to initialize and deploy the infrastructure:  
   ```bash
   terraform init  
   terraform apply  
   ```

4. **Commit the State File:**  
   - Once the configuration is applied, commit the `terraform.tfstate` file to your repository.  
   - Your AWS Organization setup is now complete! 🎉  
