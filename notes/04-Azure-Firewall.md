# Azure Firewall

## 1. Introduction

Azure Firewall is a managed, cloud-based network security service designed to protect Azure network resources.

It provides centralized traffic inspection and filtering.

Azure Firewall can help control:

- Inbound traffic
- Outbound traffic
- East-west traffic
- Application traffic
- Network traffic

---

# 2. Why Azure Firewall?

NSGs are useful for subnet and network interface-level filtering.

Azure Firewall provides centralized security controls across network environments.

A common architecture is:

```text
Spoke VNet
    |
    v
Hub VNet
    |
    v
Azure Firewall
    |
    v
Internet
