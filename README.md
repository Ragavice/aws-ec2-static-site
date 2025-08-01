# AWS EC2 Static Website Project

## Summary
Launched an EC2 instance using Ubuntu and deployed a simple static website with Nginx.

## EC2 Configuration
- Instance type: t2.micro (Free Tier)
- OS: Ubuntu Server 22.04 LTS
- Ports allowed: 22 (SSH), 80 (HTTP)
- Web server: Nginx

## Deployment
- A simple HTML page was deployed to `/var/www/html/index.html`
- Accessible at: http://<your-ec2-public-ip>

## Commands Used
```bash
sudo apt update && sudo apt install nginx -y
echo "<h1>Hello from Ragavi!</h1>" | sudo tee /var/www/html/index.html
sudo systemctl restart nginx
