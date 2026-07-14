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
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5d2644b9-8782-4200-9a84-abb867008853" />

---

# 📷 Project Screenshots

## 1️⃣ EC2 Instance Successfully Running

The EC2 instance was launched using Ubuntu Linux and configured with a public IP address.

![EC2 Instance]
<img width="1470" height="832" alt="Screenshot 2026-07-15 at 12 00 31 AM" src="https://github.com/user-attachments/assets/10b3a0a3-7c2a-405f-bb90-9d9c2ffabd36" />

---

## 2️⃣ Connecting to EC2 Instance Using SSH

Secure Shell (SSH) was used to remotely access the Ubuntu server.

```bash
ssh -i key.pem ubuntu@PUBLIC_IP
```

![SSH Connection]
<img width="1470" height="956" alt="Screenshot 2026-07-14 at 11 48 25 PM" src="https://github.com/user-attachments/assets/6ac10469-19b2-4c4a-8257-97ca10e63ae0" />

---

## 3️⃣ Installing Apache Web Server

Apache HTTP Server was installed using Ubuntu package manager.

```bash
sudo apt update
sudo apt install apache2 -y
```

![Apache Installation]
<img width="1470" height="831" alt="Screenshot 2026-07-14 at 11 48 58 PM" src="https://github.com/user-attachments/assets/dabddf88-ed62-4fc4-b769-d6a11955de4d" />

---

## 4️⃣ Managing Website Files

The default web root directory was accessed to modify the webpage content.

```bash
cd /var/www/html
ls -la
```

The default index.html file was edited with custom HTML code.

![Website Files]
<img width="1470" height="830" alt="Screenshot 2026-07-15 at 12 14 08 AM" src="https://github.com/user-attachments/assets/945f9c96-4b56-4c1f-9145-defabc9bdcf8" />

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

![Apache Status]
<img width="1165" height="333" alt="Screenshot 2026-07-14 at 11 57 18 PM" src="https://github.com/user-attachments/assets/eba5bb01-55a1-440b-8473-5849092383e1" />

---

## 6️⃣ Final Website Output

The custom webpage was successfully deployed and accessed through the EC2 Public IPv4 Address.

![Website Output]
<img width="1470" height="838" alt="Screenshot 2026-07-14 at 11 49 45 PM" src="https://github.com/user-attachments/assets/4cdad3ce-6262-463d-8bfa-603e1e1bacae" />

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
