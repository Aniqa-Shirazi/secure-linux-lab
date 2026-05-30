# Day 1 - Linux Security Lab Notes

## 🧠 Overview

Day 1 focused on setting up a secure Linux environment using Ubuntu Server in a virtualized lab. The objective was to build foundational understanding of system identity, networking, service management, and basic security posture.

---

## 🖥️ System Identity Concepts

### Commands Used
- whoami
- hostname
- pwd
- uname -a

### Explanation

These commands help identify and verify the system environment:

- `whoami` → confirms the current logged-in user. Important for privilege awareness in security contexts.
- `hostname` → identifies the machine name within a network environment. Useful for tracking systems in multi-host environments.
- `pwd` → shows the current working directory, ensuring correct file system navigation.
- `uname -a` → provides kernel and system information, useful for system fingerprinting and vulnerability assessment.

---

## 🌐 Networking Fundamentals

### Commands Used
- ip a
- ping -c 4 google.com

### Explanation

Networking commands help validate connectivity and system communication:

- `ip a` → displays network interfaces and assigned IP addresses. Essential for understanding system exposure in a network.
- `ping` → tests connectivity and DNS resolution. Helps verify whether the system can reach external networks.

---

## 📦 Package Management (System Updates)

### Commands Used
- sudo apt update
- sudo apt upgrade -y
- sudo apt install openssh-server -y

### Explanation

Package management ensures system security and software availability:

- `apt update` → refreshes package lists from repositories (does not install updates).
- `apt upgrade` → installs available updates and security patches.
- `openssh-server` → installs SSH service for secure remote access.

Keeping systems updated is a critical cybersecurity practice to reduce vulnerabilities.

---

## 🔐 SSH Service Management

### Commands Used
- systemctl status ssh
- sudo systemctl start ssh
- sudo systemctl enable ssh

### Explanation

SSH (Secure Shell) is a secure remote access protocol:

- `systemctl status ssh` → checks whether the SSH service is running.
- `start ssh` → manually starts the service.
- `enable ssh` → ensures SSH starts automatically on boot.

SSH is a primary tool used in server administration and cybersecurity operations.

---

## 🔎 Port and Service Monitoring

### Commands Used
- ss -tuln | grep :22

### Explanation

This command checks if SSH is actively listening on port 22.

- Port 22 is the default port for SSH.
- "LISTEN" state confirms the service is active and accepting connections.

This is a basic form of service exposure verification used in security auditing.

---

## 🔥 Firewall Awareness

### Commands Used
- sudo ufw status

### Explanation

UFW (Uncomplicated Firewall) is used to manage firewall rules in Ubuntu.

- It helps control inbound and outbound network traffic.
- Checking status ensures whether firewall protection is active or not.

Firewall configuration is a key layer in system hardening.

---

## 🧪 System Monitoring (Intro Level)

### Commands Observed
- ps aux
- top

### Explanation

These commands provide visibility into running processes:

- `ps aux` → shows all active processes in the system.
- `top` → provides real-time system resource usage.

These are essential tools for system diagnostics and security monitoring.

---

## 🧭 Key Learning Outcome

By completing Day 1, I achieved:

- Understanding of Linux system identity
- Basic networking verification skills
- SSH service setup and management
- Awareness of open ports and services
- Introduction to system monitoring
- Exposure to Linux-based security fundamentals

---

## 🔐 Security Insight

Even in a basic setup, system exposure begins at:
- open ports
- running services
- network interfaces

---

## 🧠 System Understanding

Focused on building system-level awareness in Linux by analyzing identity, filesystem, processes, services, and networking.

---

## 📁 Filesystem Structure

Commands:
- pwd
- ls
- ls -la
- cd

Key learning:
- Linux uses a hierarchical filesystem
- `/` is root directory
- `/home` contains user data
- hidden files start with `.`

---

## 💾 System Resources

Commands:
- df -h (disk usage)
- free -h (memory usage)

Insights:
- disk usage shows storage health
- memory usage shows system performance
- available memory is more important than free memory in Linux

---

## ⚙️ Process Monitoring

Commands:
- ps aux
- top

Learning:
- processes represent running programs
- system continuously runs background services
- resource usage helps identify system load

---

## 🔧 Service Management

Command:
- systemctl status ssh

Insight:
- Linux services run in background
- SSH service must be active for remote access
- systemctl controls service lifecycle

---
🔥 7. FIREWALL (UFW)
🔍 Check firewall status
sudo ufw status
🔓 Allow SSH
sudo ufw allow ssh
🔥 Enable firewall
sudo ufw enable
🔐 Security relevance:

Blocks unauthorized network access.

📡 8. WIRESHARK / NETWORK TRAFFIC
🌐 Generate traffic
ping -c 4 google.com
✔ Purpose:

Creates ICMP packets for network analysis.

🧠 Packet types observed in Wireshark:
ICMP

Used for ping requests

DNS

Used for domain resolution

TCP

Used for communication sessions

Understanding and controlling these is the foundation of cybersecurity engineering.
