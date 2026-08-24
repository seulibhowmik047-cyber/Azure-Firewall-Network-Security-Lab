# Service Endpoint vs Private Endpoint

## 1. Introduction

Azure provides different methods to secure connectivity between Virtual Networks and Azure platform services.

Two important technologies are:

- Service Endpoints
- Private Endpoints

They are related but work differently.

---

# 2. Service Endpoint

A Service Endpoint allows a subnet to access supported Azure services over the Azure backbone.

The service continues to use its public endpoint.

Example:

```text
VNet
 |
Subnet
 |
Azure Backbone
 |
Storage Public Endpoint
 |
Storage Account
