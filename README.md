## Architecture Diagram

User → NGINX (EC2) → Dashboard UI
                 ↓
            Bash Script
                 ↓
              cpu.txt
                 ↓
           Linux EC2 System

Architecture diagram of a cloud-based AWS EC2 Tax Portal monitoring system. The system uses an NGINX web server hosted on an Amazon Linux EC2 instance to serve a web dashboard. A Bash script runs on the Linux system to collect real-time CPU usage metrics, which are written to a file (cpu.txt). The frontend dashboard uses JavaScript to fetch and display live system performance data every 2 seconds. The system demonstrates Linux automation, server monitoring, and AWS EC2 deployment with security group configuration for HTTP access.

## AWS Tax Portal System – Cloud Monitoring & Infrastructure Observability
# Overview

This project simulates a cloud-hosted tax portal system deployed on AWS EC2, designed to demonstrate real-time system monitoring, infrastructure automation, and web server configuration using Linux-based tooling.

The system implements a lightweight observability layer that captures system performance metrics and serves them through a web-based dashboard.

## Business Problem

# Cloud-hosted systems require:

Real-time system monitoring
Infrastructure visibility
Server health tracking
Lightweight observability solutions
Secure web access to system metrics

## This project simulates a basic production monitoring environment.

AWS Architecture
Amazon EC2 used as compute and hosting layer
Amazon Linux used for system-level operations
AWS Security Groups control HTTP access
NGINX used as web server layer
## System Architecture
NGINX serves web dashboard and static files
Bash script collects system metrics (CPU usage)
Metrics are stored in cpu.txt
JavaScript frontend polls data every 2 seconds
EC2 provides full Linux system environment
## Key Features
Real-time CPU monitoring system
Automated Bash-based data collection
Web-based dashboard with live updates
NGINX reverse web serving
Linux system administration and configuration
AWS EC2 deployment with security configuration
## Technical Skills Demonstrated
AWS EC2 provisioning and management
Linux system administration (Amazon Linux)
Bash scripting and automation
NGINX web server configuration
System monitoring and observability design
AWS security group configuration
Debugging infrastructure deployment issues
## Challenges & Solutions
Identified correct package manager (yum vs apt)
Resolved NGINX installation and service startup issues
Fixed file path errors in web server configuration
Configured AWS security groups for HTTP access
Debugged external access and browser connectivity issues
## Architecture Decisions
Bash scripting chosen for lightweight real-time monitoring
NGINX used for efficient static file serving
EC2 used for full system control and flexibility
File-based metric storage used for simplicity and transparency
JavaScript polling used for real-time UI updates
## What This Project Demonstrates
Real Linux system operations in cloud environment
Infrastructure monitoring and observability design
End-to-end EC2 deployment lifecycle
Web server configuration and troubleshooting
Practical DevOps-style thinking

