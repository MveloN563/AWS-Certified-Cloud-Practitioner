# 🖥️ EC2 & Compute

## What is EC2?
Elastic Compute Cloud — resizable virtual servers ("instances") in AWS.

## Key Concepts
| Term | Meaning |
|------|---------|
| AMI | Amazon Machine Image — template for the instance |
| Instance type | CPU/memory profile (e.g., `t3.micro`) |
| Key pair | SSH credentials for login |
| Security group | Virtual firewall at instance level |
| Elastic IP | Static public IPv4 address |

## Pricing Models
- **On-Demand** — pay per second/hour, no commitment
- **Reserved** — 1–3 year commitment, up to 72% cheaper
- **Spot** — bid on spare capacity, up to 90% cheaper
- **Savings Plans** — flexible commitment-based discount

## Other Compute Services
- **Lambda** — serverless, event-driven functions
- **ECS / EKS** — container orchestration
- **Fargate** — serverless containers
- **Elastic Beanstalk** — PaaS for app deployment
