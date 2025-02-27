#Three-Tier-Architecture
---
#🏗️This project is currently in progress
---
## **Project Structure**
```bash
Three-Tier-Architecture/
│── modules/                  # Reusable Terraform modules
│   ├── network/              # VPC, Subnets, Security Groups
│   ├── database/             # RDS PostgreSQL
│   ├── compute/              # ECS, EC2 (possibly)
│   ├── ecr/                  # ECR repositories
│   ├── monitoring/           # Prometheus, Grafana
│   ├── authentication/       # Authelia setup
│── environments/             # Environment-specific configurations
│   ├── dev/                  # Development environment
│   ├── staging/              # Staging environment
│   ├── production/           # Production environment
│── Gitlab/                    # GitLab CI/CD Pipelines
│── scripts/                  # Helper scripts (e.g., Packer, Ansible)
│── Global/                   # Global settings (e.g., IAM roles, S3 backend)
│── main.tf                   # Main entry point
│── variables.tf               # Variables for modules
│── terraform.tfvars           # Actual values for variables
│── backend.tf                 # S3 + DynamoDB state backend
│── outputs.tf                 # Output values (e.g., ALB DNS, RDS endpoint)
│── providers.tf               # AWS provider and authentication
└── README.md                  # Documentation
```
