It looks like your usage section has a few issues in the commands. Specifically, the `terraform apply` command is missing, and there's a redundant `terraform plan` after the `apply` step. Here's the corrected version:

```markdown
# Terraform VPC and Security Groups for EKS Cluster

This Terraform configuration sets up a VPC, subnets, route tables, and security groups for an EKS cluster.

## Resources Created:
- VPC with 2 public and 2 private subnets.
- Internet Gateway (IGW) for internet access.
- NAT Gateway for private subnet outbound traffic.
- Route tables for public and private subnets with appropriate routes.
- Security groups for ALB and backend nodes (EKS node group).

## Usage:
1. Initialize Terraform:
   ```bash
   terraform init
   ```

2. Create an execution plan:
   ```bash
   terraform plan
   ```

3. Apply the plan to create resources:
   ```bash
   terraform apply
   ```
```