# Network Security Overview

## 1. Introduction

Network security is the practice of protecting networks, systems, applications, and data from unauthorized access, attacks, misuse, and disruption.

In Azure, network security is implemented using multiple layers of controls such as:

- Virtual Networks (VNet)
- Subnets
- Network Security Groups (NSG)
- Application Security Groups (ASG)
- Azure Firewall
- Service Endpoints
- Private Endpoints
- User Defined Routes (UDR)
- Microsoft Entra Private Access
- Azure Network Watcher

The goal is to follow a defense-in-depth and Zero Trust approach.

---

## 2. Common Network Security Problems

Organizations commonly face the following network security issues:

### 2.1 Exposed Subnets

A subnet without appropriate security controls can expose workloads to unwanted traffic.

Example:

```text
Internet
   |
   v
Unprotected Subnet
   |
   +-- Server
   +-- Application
   +-- Database
