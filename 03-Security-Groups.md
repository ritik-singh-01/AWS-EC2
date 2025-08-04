# 🔐 Configure Security Groups in EC2

Security Groups act as virtual firewalls for your EC2 instances. They control inbound and outbound traffic based on rules you define.

---

## 🧱 What Is a Security Group?

- A security group is associated with EC2 instances
- It contains rules that allow or deny traffic
- Rules are **stateful**: if you allow inbound traffic, the response is automatically allowed

---

## ⚙️ Steps to Configure a Security Group

### 1️⃣ Create or Select a Security Group
- During EC2 launch, choose an existing group or create a new one

### 2️⃣ Define Inbound Rules
Specify which traffic can reach your instance:
| Protocol | Port | Source | Purpose |
|----------|------|--------|---------|
| SSH      | 22   | My IP  | Linux terminal access |
| HTTP     | 80   | 0.0.0.0/0 | Web server access |
| HTTPS    | 443  | 0.0.0.0/0 | Secure web access |
| RDP      | 3389 | My IP  | Windows remote access |

### 3️⃣ Define Outbound Rules
- By default, all outbound traffic is allowed
- You can restrict it if needed for compliance

### 4️⃣ Save and Attach
- Save the security group
- Attach it to your EC2 instance during launch or modify later

---

## 🛡️ Best Practices

- ✅ Use **"My IP"** for SSH/RDP to restrict access
- ✅ Avoid opening ports to `0.0.0.0/0` unless necessary
- ✅ Use separate security groups for different roles (e.g., web server, database)
- ✅ Regularly audit and clean up unused rules

---

## 💡 Example Use Case

**Web Server Configuration**  
For a public-facing web server:
- Allow HTTP (80) and HTTPS (443) from anywhere
- Allow SSH (22) only from your IP

---

## 🎓 Certification Tips

- Understand how security groups differ from NACLs (Network ACLs)
- Know how to configure rules for different use cases
- Key topic for:
  - 🧠 AWS Certified Solutions Architect – Associate
  - 🛠️ AWS Certified SysOps Administrator – Associate

---
