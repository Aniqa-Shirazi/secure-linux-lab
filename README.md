# Secure Linux Lab

## 🛡️ Cybersecurity Portfolio Project – Linux Security Foundations

This project demonstrates practical hands-on skills in Linux system administration, networking fundamentals, and basic security hardening using a virtualized lab environment.

It is part of a structured cybersecurity learning roadmap focused on SOC, cloud security, and DevSecOps foundations.

---

## 🎯 Objectives

- Build and manage a Linux server environment
- Understand networking fundamentals (IP, ports, DNS, TCP/IP)
- Configure SSH remote access securely
- Apply basic firewall rules using UFW
- Analyze system processes and logs
- Develop documentation and scripting habits

---

## 🧰 Technology Stack

- VirtualBox (Virtualization)
- Ubuntu Server LTS (Linux OS)
- OpenSSH (Remote access)
- UFW (Firewall)
- Wireshark (Network analysis)
- Git & GitHub (Version control)
- Bash scripting (Automation)

---

## 🏗️ Lab Architecture

Windows Host Machine
│
├── VirtualBox
│   └── Ubuntu Server VM
│       ├── SSH Server
│       ├── Firewall (UFW)
│       ├── System Logs
│       ├── Bash Scripts
│       └── Security Configurations
│
├── Wireshark
│   └── Network Traffic Analysis
│
├── VS Code
│   └── Script & Configuration Management
│
└── Git + GitHub
    └── Version Control & Portfolio Hosting

---

## 📅 Progress Overview

### Day 1 – System Setup & Security Baseline

**Completed Tasks:**
- VirtualBox installation and Ubuntu Server VM setup
- System update and package upgrade
- SSH server installation and verification
- Firewall status check (UFW)
- Network connectivity validation
- Basic Linux command execution

---

## 🔐 Security Implementations

- SSH service enabled and running on port 22
- System packages updated for security patches
- Basic firewall inspection (UFW)
- Network port monitoring via `ss`

---

## 🧪 Key Commands Practiced

- `whoami`
- `hostname`
- `ip a`
- `ping`
- `apt update && apt upgrade`
- `systemctl status ssh`
- `ss -tuln`
- `ufw status`

---

## 📌 Learning Outcomes

By completing this lab, I gained:

- Practical Linux server handling experience
- Understanding of SSH-based remote access
- Awareness of open ports and network services
- Exposure to system hardening concepts
- Initial experience with security documentation practices

---

## 🚀 Future Improvements

- SSH key-based authentication
- Fail2Ban integration
- Advanced firewall rules
- Log monitoring scripts (Python/Bash)
- Network traffic analysis with Wireshark
- System auditing automation

---

## 📎 Notes

This project will evolve across multiple phases as part of a cybersecurity learning roadmap targeting SOC Analyst and Cloud Security roles.
