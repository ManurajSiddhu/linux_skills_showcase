# 🐧 Linux Basic Commands Guide

This document contains the most important Linux commands that every **System Administrator / DevOps Engineer** must know.

---

## 📂 File and Directory Commands

| Command | Description | Example |
|--------|-------------|---------|
| `pwd` | Show current directory path | `pwd` |
| `ls` | List files and directories | `ls -l` |
| `cd` | Change directory | `cd /etc` |
| `mkdir` | Create directory | `mkdir projects` |
| `rmdir` | Remove empty directory | `rmdir test` |
| `touch` | Create empty file | `touch file.txt` |
| `cp` | Copy files/directories | `cp a.txt b.txt` |
| `mv` | Move or rename files | `mv old.txt new.txt` |
| `rm` | Remove files | `rm file.txt` |
| `rm -rf` | Force remove directory | `rm -rf folder/` |

---

## 📄 File Viewing Commands

| Command | Description | Example |
|--------|-------------|---------|
| `cat` | View file content | `cat file.txt` |
| `less` | Scroll file content | `less /var/log/messages` |
| `head` | View first lines | `head -n 10 file.txt` |
| `tail` | View last lines | `tail -n 20 file.txt` |
| `tail -f` | Live log monitoring | `tail -f /var/log/syslog` |

---

## 🔍 Searching Commands

| Command | Description | Example |
|--------|-------------|---------|
| `find` | Search files by name | `find /home -name "*.sh"` |
| `grep` | Search text inside file | `grep "error" log.txt` |
| `wc` | Count lines/words | `wc -l file.txt` |

---

## 👤 User and Permission Commands

| Command | Description | Example |
|--------|-------------|---------|
| `whoami` | Show current user | `whoami` |
| `id` | User UID/GID info | `id siddhu` |
| `chmod` | Change permissions | `chmod 755 script.sh` |
| `chown` | Change ownership | `chown user:user file.txt` |

---

## ⚙️ Process Management

| Command | Description | Example |
|--------|-------------|---------|
| `ps` | Show running processes | `ps aux` |
| `top` | Live system monitoring | `top` |
| `kill` | Kill process by PID | `kill 1234` |
| `uptime` | System running time | `uptime` |

---

## 💾 Disk and Memory Commands

| Command | Description | Example |
|--------|-------------|---------|
| `df -h` | Disk usage | `df -h` |
| `du -sh` | Folder size | `du -sh /var/log` |
| `free -m` | Memory usage | `free -m` |
| `lsblk` | List block devices | `lsblk` |

---

## 🌐 Networking Basics

| Command | Description | Example |
|--------|-------------|---------|
| `ping` | Check connectivity | `ping google.com` |
| `ip a` | Show IP address | `ip a` |
| `ss -tulnp` | Check open ports | `ss -tulnp` |
| `curl` | Test URL/API | `curl ifconfig.me` |

---

## 📦 Package Management (RHEL/CentOS)

| Command | Description | Example |
|--------|-------------|---------|
| `yum install` | Install package | `yum install nginx` |
| `yum remove` | Remove package | `yum remove httpd` |
| `yum update` | Update system | `yum update -y` |

---

## 🔥 Service Management (systemd)

| Command | Description | Example |
|--------|-------------|---------|
| `systemctl start` | Start service | `systemctl start nginx` |
| `systemctl stop` | Stop service | `systemctl stop nginx` |
| `systemctl status` | Check service status | `systemctl status sshd` |
| `systemctl enable` | Enable at boot | `systemctl enable nginx` |



