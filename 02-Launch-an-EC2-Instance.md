#  Launch an EC2 Instance

Learn how to launch and connect to an EC2 instance. This step-by-step guide covers the essential steps to get your instance up and running.

---

##  Steps to Launch an Instance

### 1️⃣ Sign in to AWS Management Console
- Go to [AWS Console](https://aws.amazon.com/console/)
- Navigate to the **EC2 Dashboard**

### 2️⃣ Launch Instance
- Click **"Launch Instance"** to start the instance creation wizard

### 3️⃣ Choose AMI
Select an Amazon Machine Image (AMI). Common options include:
- Amazon Linux 2
- Ubuntu Server
- Microsoft Windows Server

### 4️⃣ Choose Instance Type
Select the instance type based on your requirements:
- `t3.micro` – Low-cost testing (Free Tier eligible)
- `c5.large` – Compute-intensive
- `r5.large` – Memory-intensive

### 5️⃣ Configure Instance
- Set up network settings
- Assign IAM roles
- Configure advanced options if needed

### 6️⃣ Add Storage
- Attach Elastic Block Store (EBS) volumes
- Modify default volume size and type

### 7️⃣ Add Tags
- Apply tags to organize and identify instances  
  Example: `Name: MyWebServer`

### 8️⃣ Configure Security Group
- Define inbound/outbound rules  
  Example:
  - Allow SSH (port 22)
  - Allow HTTP (port 80)

### 9️⃣ Review and Launch
- Review all settings
- Click **"Launch"**
- Select an existing key pair or create a new one

---

## 🔗 Connecting to Your Instance

### 🐧 Linux (SSH)
```bash
ssh -i "your-key.pem" ec2-user@your-instance-public-dns
Windows: Use Remote Desktop (RDP). Download the RDP file and use the password generated during instance launch.

Example Use Case
Development: Developers use EC2 instances to test new applications before deploying them to production.

Certification Tips
Practice launching and configuring instances: Key for the AWS Certified Solutions Architect and AWS Certified DevOps Engineer exam
