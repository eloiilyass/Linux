# 🐧 Linux Server Lab — Ubuntu Server Deployment & Administration

> **Ubuntu Server 22.04 · Linux CLI · OpenSSH · Apache · VMware · Network Administration**

![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Ubuntu%20Server%2022.04-E95420?style=flat-square&logo=ubuntu)
![Tool](https://img.shields.io/badge/Virtualization-VMware%20Workstation-607078?style=flat-square)
![Type](https://img.shields.io/badge/Lab-Linux%20Server%20Simulation-orange?style=flat-square)

---

## 📌 Overview

This project demonstrates a **complete Linux server deployment workflow** in a virtualized enterprise environment.

It covers the full pipeline from OS installation to production-ready services: system configuration, network verification, secure SSH remote access, and Apache web server deployment — directly applicable to **Linux Administrator**, **IT Support**, and **Junior Sysadmin** roles.

---

## 🧱 Lab Architecture

| Component | Details |
|---|---|
| Server | Ubuntu Server 22.04 LTS |
| Client | Windows 10 (SSH access) |
| Virtualization | VMware Workstation |
| Remote Access | OpenSSH |
| Web Service | Apache HTTP Server |

---

## ⚙️ Technologies & Tools

`Ubuntu Server 22.04` · `Linux CLI (Bash)` · `OpenSSH` · `Apache Web Server` · `apt` · `VMware Workstation` · `Network Configuration` · `ping` · `ip addr`

---

## 🗂️ Project Structure

```
Lab
├── Part 1 — VM Setup & Ubuntu Server Installation
├── Part 2 — Initial System Configuration & Networking
├── Part 3 — Remote Access via SSH
└── Part 4 — Apache Web Server Deployment & Testing
```

---

## 🔹 Part 1 — Installation & Setup

Created a virtual machine in VMware Workstation, loaded Ubuntu Server 22.04 ISO, and completed the full OS installation.

> 📸 **Screen 1** — VMware VM creation and ISO loading

![VM Setup](./linux-setup.png)

> 📸 **Screen 2** — Ubuntu Server installation in progress

![Installation](./09-installing.png)

---

## 🔹 Part 2 — Initial Configuration

Performed all post-installation steps to prepare the server for production use:

| Step | Command / Action | Result |
|---|---|---|
| First login | Credential authentication | ✅ Access granted |
| System update | `sudo apt update && apt upgrade` | ✅ Packages updated |
| IP address check | `ip addr` | ✅ IP assigned |
| Connectivity test | `ping 8.8.8.8` | ✅ Internet reachable |

> 📸 **Screen 3** — First login to Ubuntu Server

![Login](./01-login.png)

> 📸 **Screen 4** — System packages updated via apt

![Update](./02-update.png)

> 📸 **Screen 5** — IP address verified

![IP](./03-ip.png)

> 📸 **Screen 6** — Internet connectivity confirmed via ping

![Ping](./04-ping.png)

---

## 🔹 Part 3 — Remote Access (SSH)

Enabled and tested **secure remote administration** from a Windows 10 client to the Ubuntu Server over SSH.

- Protocol: OpenSSH
- Direction: Windows 10 → Ubuntu Server
- Result: ✅ Successful remote session established

> 📸 **Screen 7** — SSH connection from Windows client to Linux server

![SSH](./ssh-connection.png)

---

## 🔹 Part 4 — Web Server Deployment (Apache)

Installed and configured Apache HTTP Server, then validated the service from a remote browser:

```bash
sudo apt install apache2
sudo systemctl enable apache2
sudo systemctl start apache2
```

| Test | Result |
|---|---|
| Apache service status | ✅ Active & running |
| Web access from browser | ✅ Default page loaded |

> 📸 **Screen 8** — Apache installation via apt

![Apache Install](./apache-install.png)

> 📸 **Screen 9** — Web server default page accessed from client browser

![Web](./web-test.png)

---

## ✅ Key Achievements

- Deployed a **Ubuntu Server 22.04** environment from scratch in VMware
- Performed complete **post-installation configuration** (updates, networking)
- Enabled and validated **SSH remote access** from a Windows client
- Installed and tested a fully operational **Apache web server**
- Verified **end-to-end connectivity** at each stage of deployment

---

## 🎯 Skills Demonstrated

| Category | Skills |
|---|---|
| Linux Administration | Ubuntu Server, Bash CLI, apt, systemctl |
| Remote Management | OpenSSH, client-server authentication |
| Web Services | Apache HTTP Server, service management |
| Networking | IP configuration, DNS, ping, connectivity testing |
| Virtualization | VMware Workstation, VM provisioning |

---

## 💼 Target Roles

This project directly demonstrates skills required for:

- **Linux System Administrator**
- **IT Support Technician**
- **Junior DevOps / Sysadmin**

---

*Lab built in an isolated VMware environment — all configurations documented with screenshots and test results.*
