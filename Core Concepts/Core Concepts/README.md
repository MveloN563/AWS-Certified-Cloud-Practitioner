# 📘 Core Concepts

Foundational AWS topics covered during the re/Start program. Each file
contains structured notes, key terms, and practical relevance.

| Topic | File |
|-------|------|
| EC2 & Compute | [EC2-and-Compute.md](./EC2-and-Compute.md) |
| Linux | [Linux.md](./Linux.md) |
| Networking | [Networking.md](./Networking.md) |
| ML & GenAI | [ML-and-GenAI.md](./ML-and-GenAI.md) |
| WordPress | [WordPress.md](./WordPress.md) |

---

## AWS Shared Responsibility Model

- **AWS is responsible for:** security *of* the cloud (physical
  infrastructure, hardware, managed services).
- **Customer is responsible for:** security *in* the cloud (data, IAM,
  patching guest OS, security groups).

---

## AWS Global Infrastructure

- **Regions** — geographic areas (e.g., `us-west-2`)
- **Availability Zones (AZs)** — isolated data centres within a Region
- **Edge Locations** — CDN endpoints for CloudFront
