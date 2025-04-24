# 🌐 Load Balanced Web Server Lab (Ubuntu Linux)

This lab demonstrates the configuration of a scalable web infrastructure using three Ubuntu-based virtual machines (VMs) and a load balancer. It simulates real-world deployment practices for high availability and traffic distribution.

## ⚙️ Lab Setup

- **VM1**: Load Balancer (`Nginx`)
- **VM2**: Web Server 1 (`Apache` or `Nginx`)
- **VM3**: Web Server 2
- **VM4**: Web Server 3 (optional or used for failover testing)

## 📁 Files

- `load_balancer_config.txt`: Sample Nginx config file
- `Screenshots/`: Setup and verification images

## 🚀 What Was Done

1. Installed and configured web servers on all VMs with unique HTML landing pages.
2. Installed and configured a load balancer on VM1 to distribute traffic using round-robin.
3. Verified setup using:
   - `curl` to simulate traffic distribution
   - Browser tests showing load balancing in action
   - Screenshots showing server responses and status

## 🛠️ Key Commands Used

```bash
# Install Nginx
sudo apt update && sudo apt install nginx

# Configure load balancer (example)
sudo nano /etc/nginx/sites-available/default

# Restart Nginx
sudo systemctl restart nginx
