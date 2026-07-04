# Terraform AWS Infrastructure

Provision AWS infrastructure using **Terraform** with a modular architecture, reusable modules, and remote state management using **Amazon S3**.

This project demonstrates the fundamentals of **Infrastructure as Code (IaC)** by provisioning AWS resources through Terraform while following a modular project structure.

---

## Project Overview

This project was built as part of my DevOps learning journey to understand Infrastructure as Code using Terraform.

The project provisions AWS resources using reusable modules and demonstrates:

- Infrastructure provisioning using Terraform
- Modular Terraform project structure
- Variable and output management
- Remote state management using Amazon S3
- S3 bucket versioning and encryption
- Terraform state management and backend configuration

---

## Technologies Used

- Terraform
- Amazon Web Services (AWS)
- Amazon EC2
- Amazon S3
- Git
- GitHub

---

## AWS Resources Created

The project provisions the following resources:

### EC2 Module

- Amazon EC2 Instance
- Configurable AMI
- Configurable Instance Type
- Resource Tagging

### S3 Module

- Amazon S3 Bucket
- Versioning Enabled
- Server-Side Encryption (AES256)
- Public Access Block Enabled

---

## Project Structure

```
terraform-aws-infrastructure/
│
├── backend.tf
├── provider.tf
├── versions.tf
├── main.tf
├── variables.tf
├── outputs.tf
├── terraform.tfvars.example
├── README.md
├── .gitignore
│
└── modules/
    ├── ec2/
    │   ├── main.tf
    │   ├── variables.tf
    │   └── outputs.tf
    │
    └── s3/
        ├── main.tf
        ├── variables.tf
        └── outputs.tf
```

---

## Terraform Workflow

Initialize Terraform

```bash
terraform init
```

Review Infrastructure Changes

```bash
terraform plan
```

Provision Infrastructure

```bash
terraform apply
```

Destroy Infrastructure

```bash
terraform destroy
```

---

## Remote Backend

Terraform state is stored remotely in an Amazon S3 bucket.

Backend Features:

- Remote Terraform State
- Bucket Versioning Enabled
- Server-Side Encryption Enabled
- Public Access Block Enabled

This enables centralized and reliable state management while following Infrastructure as Code best practices.

---

## Learning Outcomes

Through this project I gained hands-on experience with:

- Terraform Providers
- Terraform Resources
- Variables
- Outputs
- Modules
- Terraform State File
- Remote Backend
- AWS Infrastructure Provisioning
- Infrastructure as Code (IaC)

---

## Future Enhancements

Planned improvements include:

- Security Group Module
- IAM Role Module
- User Data Automation
- Jenkins Integration
- Docker Deployment Automation
- GitOps Integration using Argo CD

---

## Screenshots

Screenshots demonstrating the infrastructure deployment will be added here.

- Terraform Apply
- AWS EC2 Instance
- Amazon S3 Bucket
- Remote State File
- Terraform Outputs

---

## Author

**Aditya M Khiroji**

GitHub: https://github.com/YOUR_GITHUB_USERNAME

LinkedIn: https://www.linkedin.com/in/YOUR_LINKEDIN_USERNAME/

---

## License

This project is licensed under the MIT License.
