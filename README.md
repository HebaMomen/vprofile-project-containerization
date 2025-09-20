# vProfile Application Containerization

![Docker](https://img.shields.io/badge/Docker-Containerized-blue)
![MySQL](https://img.shields.io/badge/MySQL-5.7-orange)
![Tomcat](https://img.shields.io/badge/Tomcat-8-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

A complete containerization solution for the vProfile application using Docker and Docker Compose.

## 📋 Project Overview

This project demonstrates containerization of a Java web application (vProfile) with:
- **MySQL 5.7** database with custom user configuration
- **Tomcat 8** application server
- **Nginx** load balancer
- **Memcached** caching service
- **RabbitMQ** message broker

## 🚀 Quick Start

### Prerequisites
- Ubuntu 20.04+ or any Linux distribution
- Docker Engine
- Docker Compose

### Installation

1. **Clone the repository**:
  
   git clone https://github.com/HebaMomen/vprofile-project-containerization.git
   cd vprofile-project-containerization
Build and run the application:


docker-compose up -d --build
Access applications:

Web Application: http://localhost:8080

RabbitMQ Management: http://localhost:15672 (username: test, password: test)

MySQL Database: localhost:3306 (username: admin, password: admin123)

📁 Project Structure
text
vprofile-project-containerization/
├── docker-configs/          # Docker configuration files
│   ├── Dockerfile.app
│   ├── Dockerfile.db
│   ├── nginx.conf
│   └── db_backup.sql
├── docker-compose.yml       # Multi-container orchestration
├── application.properties   # Application configuration
├── setup.sh                # Environment setup script
└── README.md               # Project documentation
🔧 Key Features
✅ Fixed MySQL admin user authentication issues

✅ SSL configuration for MySQL compatibility (useSSL=false&serverTimezone=UTC)

✅ Multi-container Docker Compose orchestration

✅ Nginx reverse proxy setup

✅ Custom MySQL user creation with proper privileges

✅ Ready for Kubernetes deployment

🐛 Problem Solved
This project resolves the "HTTP Status 500 - Internal Server Error" caused by:

MySQL admin user authentication failures

SSL handshake issues between Java 11 and MySQL 5.7

Database connection timezone conflicts

🛠️ Technical Stack
Database: MySQL 5.7.25

Application Server: Tomcat 8 with Java 11

Web Server: Nginx

Caching: Memcached

Message Broker: RabbitMQ

Orchestration: Docker Compose

👨‍💻 Author
Heba Momen

GitHub: @HebaMomen

Project: vProfile Containerization

📝 License
This project is licensed under the MIT License.

text

## **To use this:**

1. **Open your README.md file:**
 
   nano README.md
