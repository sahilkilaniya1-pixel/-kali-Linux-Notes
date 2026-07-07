# -kali-Linux-Notes
# 🐧 Kali Linux: Basic to Advanced Command Guide

A comprehensive, hands-on documentation of Kali Linux commands and penetration testing methodologies, structured from beginner to advanced levels. Built for quick reference during labs, CTFs, and real-world assessments.

---

## 📑 Table of Contents
1. [Linux Basics & File Management](#1-linux-basics--file-management)
2. [Permissions & System Management](#2-permissions--system-management)
3. [Networking & Log Monitoring](#3-networking--log-monitoring)
4. [Advanced Pentesting & Tooling](#4-advanced-pentesting--tooling)
5. [Git Workflow for this Repo](#5-git-workflow-for-this-repo)

---

## 1. Linux Basics & File Management

The foundation of navigating the Linux filesystem.

| Command | Description | Practical Example |
| :--- | :--- | :--- |
| `pwd` | Print Working Directory | `pwd` |
| `ls` | List directory contents | `ls -la` *(Shows details & hidden files)* |
| `cd` | Change directory | `cd /var/www/html` |
| `mkdir` | Create a new directory | `mkdir -p pentest/scans` *(Creates nested folders)* |
| `touch` | Create an empty file | `touch targets.txt` |
| `cp` | Copy files or directories | `cp exploit.py exploit_backup.py` |
| `mv` | Move or rename files | `mv targets.txt /tmp/` |
| `rm` | Remove files or directories | `rm -rf old_scans/` *(Force delete folder)* |

---

## 2. Permissions & System Management

Managing file ownership, execution rights, and administrative privileges.

### File Permissions Breakdown (`chmod`)
* **`chmod +x script.sh`** -> Makes a downloaded shell script executable.
* **`chmod 755 exploit.py`** -> Gives Full privileges to Owner, Read/Execute to others.

### System Control
* **`sudo`**: Execute a command with root privileges.
  ```bash
  sudo apt update && sudo apt upgrade -y
