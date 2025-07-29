## Overview
A hands‑on lab to explore SAP Adaptive Server Enterprise (ASE) 16.0 on AWS. Includes practical DBA tasks, performance tuning, backup/restore, and monitoring screenshots.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Architecture Diagram](#architecture-diagram)
3. [Installation & Configuration](#installation--configuration)
4. [DBA Tasks](#dba-tasks)
   - [Backup & Restore](#backup--restore)
   - [Performance Tuning](#performance-tuning)
   - [Stored Procedure Scheduling](#stored-procedure-scheduling)
5. [Monitoring & Screenshots](#monitoring--screenshots)
6. [Usage Examples](#usage-examples)
7. [License](#license)

## Prerequisites
- AWS account with IAM privileges
- EC2 instance (Ubuntu Server 22.04 LTS)
- SAP Developer ID to download ASE 16.0 trial
- Security group: SSH (22), ASE port (5000), Cockpit (8080)

## Architecture Diagram
![ASE Lab Architecture](screenshots/architecture-diagram.png)

## Installation & Configuration
1. Download and extract the ASE 16.0 developer edition.
2. Copy installer to EC2 and run:
   ```bash
   sudo ./setup_server.sh
