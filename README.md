# AWS Tax Portal System (Linux Monitoring & Cloud Deployment)

A cloud-based **Tax Portal simulation system** deployed on AWS EC2 using Linux, NGINX, and real-time system monitoring via Bash scripting.

This project demonstrates real-world cloud engineering concepts including infrastructure deployment, Linux administration, web server configuration, and system monitoring automation.

---

#  Live Architecture


User Browser
↓
NGINX Web Server (EC2)
↓
Linux Bash Monitoring Script
↓
cpu.txt (Live System Metrics)
↓
Frontend Dashboard (HTML + JS)


---

# Live System Features

- AWS EC2 hosted deployment
- NGINX web server configuration
- Real-time CPU monitoring
- Bash automation scripts
- Live dashboard UI updates (2-second refresh)
- AWS Security Group configuration
- Linux system troubleshooting & debugging

---

# Tech Stack

- AWS EC2 (Amazon Linux)
- NGINX
- Bash Scripting
- HTML / CSS / JavaScript
- Linux system tools (top, ps, systemctl)

---

#  Real Challenges & Solutions

## 1. Wrong Linux package manager
**Issue:** Used `apt` instead of `yum`

**Fix:** Learned Amazon Linux uses:
```bash
yum install
2. NGINX service missing

Issue: systemctl start nginx failed

Fix: Installed NGINX using:

sudo yum install nginx -y
3. 404 error on cpu.txt

Issue: File not found in browser

Fix: Understood NGINX serves only:

/usr/share/nginx/html/
4. AWS browser timeout

Issue: Website not accessible externally

Fix: Configured AWS Security Group:

HTTP port 80 opened to 0.0.0.0/0
🧠 Key Learnings
Linux system administration (Amazon Linux)
AWS EC2 deployment and configuration
NGINX web server setup
Bash scripting for automation
Real-time system monitoring
AWS networking and security groups
Debugging production-level infrastructure issues
 System Monitoring

# The system tracks:

CPU usage (real-time every 2 seconds)
Web server status (NGINX health)
System performance metrics

Data is generated using a Bash script and served via NGINX.

# How It Works
Bash script collects CPU usage using Linux top
Data is written to cpu.txt
NGINX serves file to web browser
JavaScript fetches updates every 2 seconds
Dashboard displays live system performance

# Screenshots
AWS Infrastructure
EC2 instance running
Security group configuration (HTTP 80 open)
Deployment
NGINX active status
Website live on public IP
Monitoring
Live CPU usage dashboard
cpu.txt output in browser
Terminal script running in background

# Future Improvements
Add RAM & Disk monitoring
Convert script to Python API (Flask)
Integrate AWS CloudWatch
Add authentication system (login page)
Deploy using Terraform (Infrastructure as Code)
Author

Temitope Ajo
AWS | Linux | Automation | Infrastructure Monitoring

📌 Project Purpose

To simulate a real-world cloud-hosted tax portal system with integrated Linux monitoring, demonstrating practical DevOps and cloud engineering skills.



