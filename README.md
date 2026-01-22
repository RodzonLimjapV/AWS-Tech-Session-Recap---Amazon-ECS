# AWS Tech Session Recap – Amazon ECS

Welcome to the recap of our recent AWS Tech Sharing session focused on **Amazon ECS (Elastic Container Service)**.

** Audience:** Developers, QA Engineers, UI/UX Designers, DevOps & Cloud Engineers
** Topic:** Modernizing application deployment using containerized architecture with Amazon ECS

---

## 1. Traditional vs Microservices Architecture

###  Traditional Architecture

Applications are built as a single, tightly coupled unit where all components are deployed together.

<img width="301" height="272" alt="image" src="https://github.com/user-attachments/assets/cd2f3ff2-6d5f-4a55-ad2c-5e327bafe86f" />


### Microservices Architecture

Applications are split into small, independent services that communicate via APIs and can be deployed individually.

* Each service can scale independently
* Enhances development speed and resilience
* One failure won't bring down the entire app
🛠️ Container technology is essential to achieving microservices at scale.

<img width="261" height="271" alt="image" src="https://github.com/user-attachments/assets/2506a019-9e9c-4a3d-b07b-f322a0228e8c" />

---

## 2. What Is a Container or Image?

Containers package code, runtime, tools, and dependencies. They are built from read-only **images**.

### ✅ Benefits:

* Portable runtime application environment
* Single, immutable deployment artifact
* Support multiple versions with different dependencies
* Faster deployments
* Efficient resource utilization

<img width="392" height="207" alt="image" src="https://github.com/user-attachments/assets/64f2ab06-bd7b-4688-8a28-6db7bff35031" />


---

## 3. What Does Amazon ECS Do?

Amazon ECS is a **fully managed container orchestration service** that lets you:

* Deploy, run, and manage containers
* Use either **EC2** or **Fargate** for compute
* Integrate with AWS services for monitoring, scaling, and security
<img width="207" height="208" alt="image" src="https://github.com/user-attachments/assets/7c23a053-fe07-4c19-a8bd-544ebebbdf2e" />

---

##  4. Key Technical Concepts

### 🔹 Cluster
A logical grouping of services or tasks. With Fargate, infrastructure is abstracted.

### 🔹 Image & Container
Containers run from immutable images (stored in **ECR**) that include all necessary code and dependencies.

### 🔹 Task Definition
Blueprint for launching containers: image, CPU/memory, environment, ports, etc.

### 🔹 Task
A running instance of a task definition. It may consist of one or more containers.

### 🔹 Service
Ensures the desired number of tasks are always running. Auto-replaces unhealthy tasks.

<img width="332" height="196" alt="image" src="https://github.com/user-attachments/assets/e41349ef-8718-4b83-a1f2-463b290b2d7c" />


     
---

## 5. Benefits of Using Amazon ECS

### ✅ Fully Managed
ECS handles the orchestration—no need to manage control plane components.

### ✅ Fargate Integration
* Serverless compute for containers
* No EC2 to manage
* Enhanced security and resource isolation

### ✅ Deep AWS Integrations
ECS connects natively with:

* Elastic Load Balancing
* CloudWatch Logs
* Secrets Manager
* Systems Manager
* CodeDeploy
* Elastic Container Registry (ECR)

---

## 6. ECS Launch Type Options

### EC2 Launch Type
* Run ECS tasks on your managed EC2 fleet
* Full infrastructure control and visibility

### Fargate Launch Type
* AWS-managed serverless infrastructure
* Focus only on task/container config
* Simplifies scaling and cost management

---

## 7. Common Use Cases

### Batch Processing
Plan, schedule, and run batch jobs using ECS with EC2/Fargate/Spot Instances.

###  Scalable Web Apps
Deploy scalable web services across multiple AZs with built-in HA and autoscaling.

###  Hybrid Deployments
Use **ECS Anywhere** for on-premise + cloud deployments with unified tooling and visibility.

---

##  8. Video Reference

A walkthrough recording and YT demo is available on YouTube: \
https://bit.ly/15MinsECS

---

## 🙌 Thank You

This document is part of the AWS Tech Sharing series. \
Stay tuned for future sessions!

---

### 📎 Resources:

* [Amazon ECS Documentation](https://docs.aws.amazon.com/ecs/)
* [ECR (Elastic Container Registry)](https://aws.amazon.com/ecr/)
* [Containers on AWS](https://aws.amazon.com/containers/)
* [AWS Fargate](https://aws.amazon.com/fargate/)
---

> 📘 *Feel free to fork this repo or submit improvements!*

---

© 2025 AWS Tech Sharing
