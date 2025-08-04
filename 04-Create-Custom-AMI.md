# 🧬 Create a Custom AMI in EC2

A custom Amazon Machine Image (AMI) allows you to save the configuration of an EC2 instance and reuse it to launch identical instances.

---

## 🧭 What Is a Custom AMI?

- A snapshot of an EC2 instance's configuration
- Includes OS, installed software, settings, and attached volumes
- Useful for scaling, backups, and environment replication

---

## ⚙️ Steps to Create a Custom AMI

### 1️⃣ Prepare Your EC2 Instance
- Install required software and updates
- Configure settings (e.g., environment variables, services)
- Clean up sensitive data (e.g., SSH keys, logs)

### 2️⃣ Create Image from EC2 Console
- Go to **EC2 Dashboard > Instances**
- Select your instance
- Click **Actions > Image > Create Image**

### 3️⃣ Fill in Image Details
- **Image Name**: e.g., `MyAppServer-AMI`
- **Description**: Optional but helpful
- Choose whether to reboot the instance during image creation

### 4️⃣ Monitor AMI Creation
- Go to **EC2 Dashboard > AMIs**
- Wait for the status to change to `available`

### 5️⃣ Launch Instances from Custom AMI
- Use your AMI to launch new EC2 instances
- All configurations will be preloaded

---

## 🛡️ Best Practices

- ✅ Remove temporary files and credentials before creating the AMI
- ✅ Use meaningful names and tags for easy identification
- ✅ Regularly update your AMIs to include patches and improvements
- ✅ Automate AMI creation using scripts or AWS Systems Manager

---

## 💡 Example Use Case

**Scaling a Web Application**  
Create a custom AMI of a configured web server and use it to:
- Launch multiple instances behind a load balancer
- Ensure consistent environment across deployments

---

## 🎓 Certification Tips

- Understand the difference between AMIs and snapshots
- Know how to create, manage, and share AMIs
- Key topic for:
  - 🧠 AWS Certified Solutions Architect – Associate
  - 🛠️ AWS Certified DevOps Engineer – Professional

---
