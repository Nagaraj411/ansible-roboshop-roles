# 🤖 Ansible Roboshop Roles

This repository contains reusable and modular **Ansible roles** to automate the deployment and configuration of the **Roboshop application** — a microservices-based e-commerce platform. Each role manages a specific service to ensure scalable, consistent, and production-ready infrastructure provisioning.

---

## 📦 Services Covered

The following components are implemented as individual Ansible roles:

| Role       | Description                                |
|------------|--------------------------------------------|
| `catalogue`| Deploys the Node.js-based product catalogue service |
| `frontend` | Configures and deploys the Nginx frontend UI |
| `user`     | Manages the user service that interacts with MongoDB |
| `cart`     | Handles cart service backed by Redis       |
| `shipping` | Deploys the shipping service using MySQL   |
| `payment`  | Deploys the payment service using Python   |
| `mongodb`  | Installs and configures MongoDB database   |
| `redis`    | Installs and configures Redis key-value store |
| `mysql`    | Installs and configures MySQL for shipping |
| `rabbitmq` | Sets up RabbitMQ for messaging between services |


---

## 🚀 How to Run

1. 📥 Clone the repository:
```bash
    git clone https://github.com/Nagaraj411/ansible-roboshop-roles.git
    cd ansible-roboshop-roles
    ▶️ Run the playbook:
    ansible-playbook -i inventory roboshop.yml
