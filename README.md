# 🚀 AWS EC2 Apache Web Server Deployment

## 📌 Project Overview

This project demonstrates the deployment of a Linux-based web server on AWS Cloud using Amazon EC2 and Apache HTTP Server.

The objective was to provision a virtual machine, configure the operating system, install a web server, and host a custom HTML webpage accessible over the internet.

This project was completed as part of the **DecodeLabs Cloud Computing Internship - Project 2 (Server Commander)**.

---

# 🎯 Objectives

- Launch an EC2 Instance on AWS
- Configure a Linux (Ubuntu) Server
- Connect securely using SSH
- Install Apache Web Server
- Host a custom HTML webpage
- Make the webpage accessible through a Public IP Address

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| AWS EC2 | Virtual Machine Hosting |
| Ubuntu Linux | Operating System |
| Apache2 | Web Server |
| SSH | Secure Remote Access |
| HTML/CSS | Webpage Development |
| AWS Security Groups | Firewall Configuration |

---

# 🏗 Architecture

```text
User Browser
      │
      ▼
Public IPv4 Address
      │
      ▼
AWS EC2 Instance (Ubuntu)
      │
      ▼
Apache Web Server
      │
      ▼
index.html
```

---

# 📷 Project Screenshots

## 1️⃣ EC2 Instance Successfully Running

The EC2 instance was launched using Ubuntu Linux and configured with a public IP address.

![EC2 Instance](screenshots/01-ec2-instance-running.png)

---

## 2️⃣ Connecting to EC2 Instance Using SSH

Secure Shell (SSH) was used to remotely access the Ubuntu server.

```bash
ssh -i key.pem ubuntu@PUBLIC_IP
```

![SSH Connection](screenshots/02-ssh-connection.png)

---

## 3️⃣ Installing Apache Web Server

Apache HTTP Server was installed using Ubuntu package manager.

```bash
sudo apt update
sudo apt install apache2 -y
```

![Apache Installation](screenshots/03-apache-installation.png)

---

## 4️⃣ Managing Website Files

The default web root directory was accessed to modify the webpage content.

```bash
cd /var/www/html
ls -la
```

The default index.html file was edited with custom HTML code.

![Website Files](screenshots/04-website-files.png)

---

## 5️⃣ Verifying Apache Service Status

Apache service was checked to ensure the server was running properly.

```bash
sudo systemctl status apache2
```

Status:

```text
active (running)
```

![Apache Status](screenshots/05-apache-status.png)

---

## 6️⃣ Final Website Output

The custom webpage was successfully deployed and accessed through the EC2 Public IPv4 Address.

![Website Output](screenshots/06-website-output.png)

---

# 📂 Project Structure

```text
aws-ec2-apache-web-server
│
├── README.md
│
├── screenshots
│   ├── 01-ec2-instance-running.png
│   ├── 02-ssh-connection.png
│   ├── 03-apache-installation.png
│   ├── 04-website-files.png
│   ├── 05-apache-status.png
│   └── 06-website-output.png
│
└── source-code
    └── index.html
```

---

# 💻 Commands Used

## Update Ubuntu Packages

```bash
sudo apt update
sudo apt upgrade -y
```

## Install Apache

```bash
sudo apt install apache2 -y
```

## Check Apache Status

```bash
sudo systemctl status apache2
```

## Restart Apache

```bash
sudo systemctl restart apache2
```

## Open Web Directory

```bash
cd /var/www/html
```

## Edit HTML File

```bash
nano index.html
```

---

# 🌐 Website Features

- Responsive webpage
- Hosted on AWS EC2
- Ubuntu Linux Server
- Apache HTTP Server
- Publicly accessible through IPv4 address

---

# 📚 Learning Outcomes

Through this project, I learned:

- Cloud Infrastructure Basics
- Amazon EC2 Management
- Linux Server Administration
- SSH Remote Connectivity
- Apache Web Server Configuration
- Hosting Static Websites
- AWS Security Groups
- Infrastructure as a Service (IaaS)

---

# 🔒 Security Configuration

The following inbound rules were configured:

| Type | Port |
|--------|--------|
| SSH | 22 |
| HTTP | 80 |

These rules allow:

- Secure server access through SSH
- Public website access through HTTP

---

# ✅ Project Outcome

Successfully deployed a Linux-based web server on AWS EC2, installed Apache HTTP Server, configured a custom webpage, and made the application accessible through a public IPv4 address.

---

# 👨‍💻 Author

**Shivam Singh**

DecodeLabs Cloud Computing Internship

Project 2 – Server Commander

AWS EC2 Apache Web Server Deployment

---
