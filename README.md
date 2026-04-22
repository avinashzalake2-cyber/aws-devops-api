
# AWS DevOps API Deployment

##  Project Overview
This project demonstrates deployment of a simple Flask API using Docker on AWS EC2.

##  Features
- Simple REST API
- Docker containerization
- Public endpoint access
- Health check endpoint

##  API Endpoints
- `/` → Returns welcome message  
- `/health` → Returns status  

##  Docker
Build:
docker build -t my-api .

Run:
docker run -d -p 5001:5000 my-api

##  AWS Deployment
- EC2 Ubuntu instance
- Port 5001 open in security group
- Docker installed and running

##  Monitoring & Logs
- Docker logs used
- EC2 basic monitoring

## Cost Estimation
- EC2 t2.micro → ~$0.01/hour  
- Daily cost ≈ $0.24 (~₹20)  
- Free tier → ₹0  

##  Public API
http://<your-ec2-public-ip>:5001
