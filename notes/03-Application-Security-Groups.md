# Application Security Groups (ASG)

## 1. Introduction

Application Security Groups (ASGs) allow Azure resources to be grouped logically based on their application or workload role.

ASGs are commonly used with Network Security Groups.

Instead of writing NSG rules using individual IP addresses, ASGs allow security rules to reference logical application groups.

---

# 2. Why ASG is Useful

Consider an environment with:

```text
Web Server 1 → 10.0.1.10
Web Server 2 → 10.0.1.11
Web Server 3 → 10.0.1.12
