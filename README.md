# Advanced AWS Networking with Terraform

A hands-on Cloud & DevOps project demonstrating Infrastructure as Code (IaC) using Terraform and AWS networking components.

## Project Overview

This repository contains Terraform configuration files for defining AWS networking infrastructure.

The project helps demonstrate how cloud infrastructure can be described, reviewed, and managed using reusable configuration rather than creating resources manually through the AWS Console.

## Technologies Used

* **Cloud Provider:** Amazon Web Services (AWS)
* **Infrastructure as Code:** Terraform
* **Configuration Language:** HashiCorp Configuration Language (HCL)
* **Version Control:** Git and GitHub

## Repository Structure

```text
terraform-aws-network-advanced/
├── main.tf
├── variables.tf
├── outputs.tf
├── .terraform.lock.hcl
├── .gitignore
└── README.md
```

* `main.tf` — Terraform resource definitions.
* `variables.tf` — Input variable declarations.
* `outputs.tf` — Output definitions.
* `.terraform.lock.hcl` — Locks selected provider dependency versions.

## Prerequisites

* An AWS account
* Terraform CLI installed
* AWS CLI installed and configured with appropriate permissions
* Basic understanding of AWS networking

## Getting Started

Clone the repository:

```bash
git clone https://github.com/akshayshendurkar55-dot/terraform-aws-network-advanced.git
```

Move into the project directory:

```bash
cd terraform-aws-network-advanced
```

Initialize Terraform:

```bash
terraform init
```

Validate the configuration:

```bash
terraform validate
```

Review the planned changes before applying anything:

```bash
terraform plan
```

Only after reviewing the plan, checking security settings, and understanding potential AWS charges should you consider creating resources.

## Security Considerations

* Restrict SSH access to trusted IP addresses instead of allowing access from `0.0.0.0/0`.
* Follow the principle of least privilege for AWS IAM permissions.
* Never commit AWS access keys, secrets, or Terraform state files to GitHub.
* Review security group rules before deploying infrastructure.

## AWS Cost Awareness

**Important:** Creating AWS networking resources can incur charges, depending on the resources and configuration used.

* Review the Terraform plan before deployment.
* Check AWS pricing and billing before creating resources.
* Remove resources that are no longer required.

After reviewing the resources created by this project, clean them up when appropriate:

```bash
terraform destroy
```

Review the destruction plan and confirm that it targets only the resources you intend to remove. Do not destroy shared or production infrastructure.

## Learning Objectives

* Understand Infrastructure as Code with Terraform
* Define AWS infrastructure through configuration files
* Validate and review infrastructure changes
* Apply security best practices to cloud networking
* Manage infrastructure lifecycle and cost awareness

## Author

Laxmikant Shendurkar

GitHub: [akshayshendurkar55-dot](https://github.com/akshayshendurkar55-dot)
