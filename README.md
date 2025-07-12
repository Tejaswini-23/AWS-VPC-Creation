# AWS VPC with Public and Private Subnets

This project demonstrates how to create a custom VPC on AWS with both public and private subnets, configured with internet access and internal routing using an Internet Gateway and a NAT Gateway.

---

## 🛠️ What’s Included

- Custom VPC (`10.0.0.0/16`)
- Public Subnet (`10.0.1.0/24`)
- Private Subnet (`10.0.2.0/24`)
- Internet Gateway (IGW)
- NAT Gateway (for private subnet internet access)
- Route Tables (for both public and private subnets)
- Optional: EC2 instances for testing connectivity

---

## 📌 Steps Followed

1. **Created VPC**
   - Name: `MyCustomVPC`
   - CIDR: `10.0.0.0/16`

2. **Created Subnets**
   - Public: `10.0.1.0/24`
   - Private: `10.0.2.0/24`

3. **Internet Gateway**
   - Created and attached to VPC

4. **Route Tables**
   - Public RT: `0.0.0.0/0 → IGW`
   - Private RT: `0.0.0.0/0 → NAT Gateway`

5. **Elastic IP & NAT Gateway**
   - EIP created and associated with NAT Gateway
   - NAT deployed in public subnet

6. **Testing**
   - EC2 instance in public subnet: direct internet access
   - EC2 instance in private subnet: internet access via NAT

---

## 📷 Screenshots

- VPC Configuration
- Subnets
- Route Tables
- IGW & NAT Gateway
- EC2 Instances

*(Add screenshots in a `screenshots/` folder and reference them here)*

---

## ✅ Outcome

- Public subnet has full internet access.
- Private subnet has outbound internet access via NAT Gateway.
- Demonstrates secure and scalable AWS VPC networking design.

---

## 📚 Technologies Used

- AWS VPC
- EC2
- Route Tables
- IGW & NAT Gateway
- Elastic IP

---

## 🧠 Author

Garaka Tejaswini  
Final-Year CSE Student  
📍 India

---

