# Day 1 - Linux Security Lab Commands

## 🖥️ System Identity Commands

whoami
hostname
pwd
uname -a

---

## 🌐 Network Verification

ip a
ping -c 4 google.com

---

## 📦 Package Management

sudo apt update
sudo apt upgrade -y
sudo apt install openssh-server -y

---

## 🔐 SSH Service Management

systemctl status ssh
sudo systemctl start ssh
sudo systemctl enable ssh

---

## 🔎 Network Port Inspection

ss -tuln | grep :22

---

## 🔥 Firewall Status Check

sudo ufw status

---

## 🧪 Optional System Monitoring

ps aux
---

## Filesystem Navigation
pwd
ls
ls -la
cd /
ls
cd ~

## System Resource Check
df -h
free -h

## Process Monitoring
ps aux | head
top

## Service Inspection
systemctl status ssh
systemctl list-units --type=service | head

## Network Awareness
ip a
ss -tuln
top
htop

# Linux Security Lab — Day 2 Commands Reference

## Objective
Day 2 focuses on process management, system services, SSH usage, logging, and basic automation.

---

# PROCESS MANAGEMENT

## View running processes
ps

Shows processes running in current shell.

---

## Detailed process list
ps aux

Displays all system processes with CPU and memory usage.

Used for:
- detecting suspicious processes
- monitoring system load

---

## Real-time process monitoring
top

Shows live CPU, memory, and process usage.

---

# SYSTEM SERVICES

## Check SSH service status
systemctl status ssh

Shows whether SSH service is active or inactive.

---

## Start SSH service
sudo systemctl start ssh

---

## Restart SSH service
sudo systemctl restart ssh

---

## List all services
systemctl list-units --type=service

---

# SYSTEM UPDATES

## Update package list
sudo apt update

---

## Upgrade system packages
sudo apt upgrade -y

---

# SSH NETWORK ACCESS

## Check IP address
ip a

Shows system IP and network interfaces.

---

## SSH login from host
ssh username@IP_ADDRESS

Used for remote secure access.

---

# SYSTEM MONITORING

## Disk usage
df -h

Shows storage usage.

---

## Memory usage
free -h

Shows RAM usage.

---

# LOGGING

## System logs
journalctl -xe

Shows system events and errors.

---

## Authentication logs
cat /var/log/auth.log

Shows login attempts and security events.

---

# BASH SCRIPT EXECUTION

## Create script
nano systeminfo.sh

---

## Make executable
chmod +x systeminfo.sh

---

## Run script
./systeminfo.sh

---

# NETWORK CHECK

## Ping test
ping google.com

---

## Network interfaces
ip a
