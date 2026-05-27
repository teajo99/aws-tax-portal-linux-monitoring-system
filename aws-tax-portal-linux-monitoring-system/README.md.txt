# ☁ AWS Tax Portal System (Linux Monitoring Project)

## 🧠 Project Overview
This project simulates a **government-style tax portal system** hosted on AWS EC2 using Linux, NGINX, and real-time system monitoring.

It started as a simple idea but evolved into a full cloud + Linux + DevOps-style project through real debugging and problem-solving.

---

## 🚀 Final Architecture

EC2 (Amazon Linux)
↓
NGINX Web Server
↓
Bash CPU Monitoring Script
↓
cpu.txt (live system data)
↓
Frontend Dashboard (HTML + JavaScript)

---

## ⚠️ Challenges I Faced (Real Mistakes)

### 1. Wrong Linux commands
I initially used:
```bash
apt update