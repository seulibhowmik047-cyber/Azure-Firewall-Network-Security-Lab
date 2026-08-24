# Azure Firewall & Network Security Lab

## Objective

This lab focuses on Azure network security concepts including:

- Network Security Groups (NSG)
- Application Security Groups (ASG)
- Azure Firewall
- Hub-and-Spoke Network Topology
- Service Endpoints
- Private Endpoints
- Microsoft Entra Private Access
- Azure Network Watcher
- Network segmentation
- Network traffic filtering

## Lab Architecture

The proposed architecture contains:

Internet
    |
Public IP
    |
Jump Server
    |
Azure Firewall
    |
Workload Subnet
    |
Internal Workload VMs

## Azure Subscription Status

This lab documentation was prepared without an active Azure subscription.
Therefore, Azure portal deployment screenshots are not available.

The repository contains the architecture, configuration plan,
security rules, commands, and implementation documentation.

## Security Objectives

1. Reduce public exposure
2. Segment workloads
3. Control inbound and outbound traffic
4. Centralize traffic inspection
5. Use private endpoints where appropriate
6. Monitor and troubleshoot network connectivity
7. Apply Zero Trust principles# Azure-Firewall-Network-Security-Lab
Hands-on Azure Network Security lab covering Azure Firewall, NSG, ASG, Private Endpoints, Entra Private Access, and Network Watcher.
