# 🧪 Linux Home Lab Setup

This project documents the setup and configuration of a personal Linux-based home lab environment, designed to simulate a small business or IT operations setting. The lab provides a safe and practical environment for experimenting with Linux system administration, user management, networking, remote access, and basic security configurations.

## 🛠️ Lab Overview

The home lab consists of:
- A **Rocky Linux 9** physical host (HP laptop)
- Multiple **VirtualBox VMs** running Ubuntu and Debian-based distributions
- A **Raspberry Pi 4** running headless Ubuntu Server

## 🧱 Lab Objectives

- Gain hands-on experience with Linux server environments
- Practice managing users, groups, and permissions
- Configure remote access and secure SSH
- Set up and manage network services
- Implement basic firewall and security policies
- Document all configurations and best practices

## 🧩 Components & Roles

| Machine              | OS / Platform     | Role                             |
|----------------------|------------------|----------------------------------|
| Rocky Linux Laptop   | Rocky Linux 9    | Host / Admin node                |
| VM 1 – Ubuntu Server | Ubuntu 22.04     | General-purpose server (SSH, Apache, users) |
| VM 2 – Debian Server | Debian 12        | Optional: file server or test environment |
| Raspberry Pi 4       | Ubuntu Server (Headless) | IoT-style device for remote management, backup, or DNS testing |

## 🔐 Features Configured

- Static IP addressing and hostname resolution
- SSH hardening (key-based auth, root login disabled)
- Custom users and groups with proper permission management
- Basic service setup (e.g., Apache, Samba, cron jobs)
- Firewalls with `ufw` and `firewalld`
- SELinux (on Rocky Linux host) for enhanced security
- System logging and basic monitoring

## 📁 Directory Structure

```bash
linux-home-lab/
├── diagrams/                # Network or system layout diagrams
├── scripts/                 # Helpful shell scripts (e.g., user creation, backups)
├── configs/                 # Sample config files (SSH, firewall, Apache)
├── notes/                   # Markdown files with detailed setup notes
└── README.md
