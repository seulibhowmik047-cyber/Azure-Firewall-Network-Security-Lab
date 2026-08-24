# VNet and Subnet Design

## VNet

Name:
test-FW-VM

Address Space:

10.0.0.0/16

## Subnets

### Workload Subnet

Name:
workload-SN

Address Space:
10.0.0.0/24

Purpose:
Hosts internal workload servers.

### Jump Subnet

Name:
jump-SN

Purpose:
Hosts the jump server used for controlled administrative access.

### Azure Firewall Subnet

Name:
AzureFirewallSubnet

Purpose:
Dedicated subnet for Azure Firewall.
