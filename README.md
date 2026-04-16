# WordPress on AWS Fargate — Terraform

Production-ready Terraform modules to deploy WordPress 
on AWS Fargate with ECS, RDS, and ALB.

## Architecture
- ECS Fargate for serverless container hosting
- RDS MySQL for database
- ALB for load balancing
- VPC with public/private subnets
- IAM roles with least-privilege policies

## Module Structure
├── modules/          # Reusable Terraform modules
├── main.tf           # Root module
├── vars.tf           # Input variables
├── outputs.tf        # Output values
├── policy.tf         # IAM policies
└── provider.tf       # AWS provider config

## Usage
1. Clone the repo
2. Update `vars.tf` with your values
3. Run `terraform init && terraform plan && terraform apply`

## Design Decisions
- [Explain WHY you chose Fargate over ECS on EC2]
- [Explain your networking choices]
- [Explain your IAM approach]
