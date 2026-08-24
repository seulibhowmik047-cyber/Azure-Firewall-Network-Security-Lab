# Hub-and-Spoke Network Topology

## 1. Introduction

Hub-and-Spoke is a network architecture where a central VNet called the Hub connects to multiple spoke VNets.

The hub provides centralized services, while the spokes contain workloads.

---

# 2. Basic Architecture

```text
                 HUB VNET
              +------------+
              | Firewall   |
              | Bastion    |
              | Shared     |
              | Services   |
              +-----+------+
                    |
       +------------+------------+
       |            |            |
       v            v            v
    Spoke 1      Spoke 2      Spoke 3
    Web/App        DB        Services
