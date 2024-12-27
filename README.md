# 🚀 Terraform AWS Infrastructure: Scalable & Modular  

Welcome to the **Terraform AWS Infrastructure Project**! This repository delivers a production-ready, scalable architecture designed with modularity and efficiency in mind. It provisions a robust environment that includes a custom VPC, public subnet, EC2 instances, and an Auto Scaling group, all powered by Terraform.

---

## 🛠️ Features  

- **Custom VPC**: Build your private cloud foundation with DNS support and hostnames enabled.  
- **Public Subnet**: Deploy highly available public subnets in your selected availability zone.  
- **EC2 Instances**: Spin up instances with configurable AMI, instance types, and tags.  
- **Auto Scaling Group**: Ensure resilience with dynamic scaling based on demand.  
- **Modular Design**: Reusable Terraform modules for effortless customization.  

---

## 📚 Project Structure

### 🗂️ Root Files:
- **`main.tf`** ➔ Root configuration integrating all modules
- **`output.tf`** ➔ Outputs for your infrastructure
- **`terraform.tfstate`** ➔ State file (auto-generated)

### 🔧 Modules:
- **`vpc/`** 🏙️: VPC module
- **`subnet/`** 🌐: Subnet module
- **`ec2/`** 💻: EC2 module
- **`autoscaling/`** 🔁: Auto Scaling module
  
---

## 🚀 Quick Start  

### 1️⃣ Prerequisites  
- **Terraform**: Install [Terraform](https://www.terraform.io/downloads.html).  
- **AWS CLI**: Configure AWS credentials with proper permissions.  

### 2️⃣ Setup  
Clone the repository and initialize Terraform:  
```bash  
git clone <repository-url>  
cd terraform-aws-infrastructure  
terraform init
```

### 3️⃣ Deploy
Run Terraform to build your infrastructure:

```bash
terraform apply  
```
Confirm and watch as your AWS environment comes to life!

### 📊 **Outputs**

- **VPC ID**: The ID of your shiny new VPC.
- **Subnet ID**: The ID of your public subnet.
- **Auto Scaling Group Name**: Name of the dynamic scaling group.
- **Instance ID**: Identifier for standalone EC2 instances.

---

🌟 **Customization**


| Variable          | Description                         | Example                   |
|-------------------|-------------------------------------|---------------------------|
| region            | AWS region                          | ap-south-1                |
| vpc_cidr_block    | CIDR block for the VPC              | 10.0.0.0/16               |
| subnet_cidr_block | CIDR block for the subnet           | 10.0.1.0/24               |
| ami               | AMI ID for EC2 instances            | ami-0dee22c13ea7a9a67     |
| instance_type     | Instance type for EC2               | t2.micro                  |

## 🤖 **Built With:**
- **Terraform**: Infrastructure as Code (IaC).
- **AWS**: Cloud infrastructure platform.

---

### 🎯 **Best Practices:**
- 🔒 **Use environment variables** for sensitive credentials.
- 📂 **Store state remotely** (e.g., S3) for collaboration.
- 🛡️ **Regularly review and restrict security group rules**.

---

**✨ Happy Terraforming! ✨**



