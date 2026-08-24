# Azure Firewall Design

## Purpose

Azure Firewall provides centralized network traffic inspection
and filtering.

## Security Controls

- Network rules
- Application rules
- FQDN filtering
- Threat intelligence
- Centralized firewall policy

## Traffic Flow

Internet
   |
   v
Jump Server
   |
   v
Azure Firewall
   |
   v
Workload Subnet
