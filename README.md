# 🚀 Containerized WordPress Application with ECS (Fargate) & RDS

I deployed a **fully containerized WordPress application** leveraging AWS managed services for **scalability, reliability, and cost efficiency**.  
This project demonstrates how modern applications can be deployed in a **cloud-native way** with **containers + serverless compute + managed databases**.

---

## 🧰 Tools & AWS Services Used

- **Amazon VPC** – Custom VPC for isolation and control  
- **Amazon ECR** – Hosted the Dockerized WordPress image  
- **Amazon ECS (Fargate)** – Ran the containerized WordPress serverlessly  
- **Amazon RDS (MySQL)** – Backend database for WordPress  
- **Application Load Balancer (ALB)** – Distributed incoming traffic  
- **AWS CLI** – For image pushes & service configuration  
- **Security Groups** – Controlled secure access between ECS tasks & RDS  

---

## 🔨 What I Built

1. Created a **custom VPC** (instead of the default VPC) with public and private subnets.  
2. Built and **pushed a local Dockerized WordPress image** to Amazon ECR.  
3. Provisioned an **RDS MySQL database** with secure credentials and networking.  
4. Configured **ECS tasks & services** to connect securely to the RDS instance.  
5. Used **security groups** to allow only the necessary ECS ↔ RDS communication.  
6. Attached an **Application Load Balancer** to route traffic to ECS tasks.  
7. Verified that the WordPress site is publicly accessible via the ALB endpoint.  

---

## 💡 Key Lessons Learned

- ✅ How to connect **ECS containers securely to RDS** inside a private VPC  
- ✅ Configuring **security groups** properly to prevent connectivity failures  
- ✅ The **workflow of local → ECR → ECS → live deployment**  
- ✅ Leveraging **Farcgate** to avoid EC2 instance management overhead  
- ✅ Understanding how **load balancing & networking** work in containerized apps  

---

## 📸 Architecture Diagram

<img width="1155" height="486" alt="diagram" src="https://github.com/user-attachments/assets/657e3d6c-b24e-4a09-b23c-d75c9ada5af8" />
<img width="1155" height="486" alt="diagram" src="https://github.com/user-attachments/assets/242ba6ef-688c-472b-ae88-86ee2c8e6d3b" />


---

## 📂 Repository Structure



