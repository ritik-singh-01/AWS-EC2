#  Amazon EC2 Quick Notes for Beginners

##  What is EC2?
Amazon EC2 (Elastic Compute Cloud): Virtual servers in the cloud to run your applications.

---

##  Key Features
- **Scalable**: Adjust server capacity as needed.
- **Flexible**: Choose instance types based on your needs.
- **Pay-as-you-go**: Pay only for what you use.

---

##  Basic Concepts
- **Instance**: A virtual server.
- **AMI**: Template with OS and software.
- **Instance Types**:
  - `t3.micro` – Small, general-purpose.
  - `c5.large` – For compute-heavy tasks.
  - `r5.large` – For memory-intensive tasks.

---

##  Pricing Models
- **On-Demand**: Pay by the hour/second. No commitment.
- **Reserved**: Save money with a 1–3 year commitment.
- **Spot**: Bid on unused capacity at lower prices.


---

##  Getting Started
1. **Choose an AMI**: Select OS/software.
2. **Pick an Instance Type**: Size your server.
3. **Set Security Groups**: Control access.
4. **Launch**: Start and connect to your instance.

---

##  Important Concepts
- **Elastic IP**: Static IP address.
- **Security Groups**: Firewall rules for your instance.
- **EBS**: Persistent storage.

---

##  Tips
- **Start Small**: Use a free tier `t3.micro` to learn.
- **Backup**: Take snapshots of your data.
- **Monitor**: Use CloudWatch for performance and cost tracking.

---

##  Resources
- **AWS Free Tier**: 750 hours/month on `t3.micro`.
- **AWS Documentation**: Learn more at [AWS Docs](https://docs.aws.amazon.com/ec2/)
