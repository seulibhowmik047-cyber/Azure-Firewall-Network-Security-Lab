# Microsoft Entra Private Access

## 1. Introduction

Microsoft Entra Private Access is a Zero Trust Network Access capability that provides identity-based access to private resources.

It is designed to reduce dependence on traditional network-level VPN access.

The key principle is:

> Users should receive access only to the resources they need.

---

# 2. Traditional VPN Model

In a traditional VPN architecture:

```text
User
 |
 v
VPN Gateway
 |
 v
Corporate Network
 |
 +-- Server 1
 +-- Server 2
 +-- Application
 +-- Database
