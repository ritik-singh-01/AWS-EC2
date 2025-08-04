# 📦 Increase EBS Volume on a Running EC2 Instance (Linux & Windows)

Need more disk space without stopping your EC2 instance? This guide walks you through increasing the size of an attached EBS volume for both Linux and Windows servers — all while the instance stays online.

---

## 🧭 Overview

- Resize EBS volumes without rebooting the instance
- Extend the file system inside the OS to utilize new space
- Applies to both Linux and Windows EC2 instances

---

## ⚙️ Step 1: Modify the EBS Volume

### 🔍 Locate the Volume
- Go to **EC2 Dashboard > Instances**
- Select your instance
- Scroll to **Storage** and note the attached volume ID

### 🛠️ Modify Volume Size
- Go to **EC2 Dashboard > Elastic Block Store > Volumes**
- Select the volume
- Click **Actions > Modify Volume**
- Enter the new size (e.g., increase from 8 GiB to 20 GiB)
- Click **Modify** and confirm

### ⏳ Monitor Status
- Volume status changes to `modifying` → `optimizing` → `completed`
- Instance remains online throughout

---

## 🐧 Step 2: Extend File System (Linux)

### ✅ Check Current Disk Usage
```bash
df -h
