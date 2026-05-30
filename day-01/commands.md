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
