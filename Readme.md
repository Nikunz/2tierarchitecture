# Terraform Infrastructure Deployment - 2tier Infrastructure #

This repository contains Terraform code to deploy a 2-tier AWS infrastructure that includes a Virtual Private Cloud (VPC), public and private subnets, security groups, EC2 instances, an Application Load Balancer (ALB), and a MySQL database instance.

## Prerequisites

Before you begin, ensure you have the following prerequisites:

1. [Terraform](https://www.terraform.io/downloads.html) installed on your local machine.
2. AWS credentials configured locally or in your environment with appropriate permissions.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. Initialize Terraform in the project directory:

   ```bash
   terraform init
   ```

3. Review and modify the `main.tf` file to match your desired configuration if necessary.

4. Deploy the infrastructure by running:

   ```bash
   terraform apply
   ```

5. Confirm the deployment by typing `yes` when prompted.

6. After the deployment is complete, Terraform will display the output values, including the ALB DNS name.

7. To destroy the infrastructure when it is no longer needed, run:

   ```bash
   terraform destroy
   ```

   Confirm the destruction by typing `yes` when prompted.

## Resources Created

This Terraform configuration will create the following AWS resources:
```
- Virtual Private Cloud (VPC)
- Public and private subnets in two availability zones
- Internet Gateway
- Route Tables and Associations
- Security Groups for EC2 instances
- EC2 instances in public subnets
- Application Load Balancer (ALB)
- ALB Listener
- Target Groups
- MySQL Database Instance in a private subnet
```
