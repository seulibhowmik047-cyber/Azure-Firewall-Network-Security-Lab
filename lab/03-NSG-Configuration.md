# 03 - NSG Rules and Application Security Groups (ASG)

## 1. Inbound Rules

Inbound rules control traffic coming **into** an Azure resource, such as a Virtual Machine.

For example, if we want to allow SSH access to a Linux VM, we can create an inbound rule that allows TCP port 22.

### Example

| Setting | Value |
|---|---|
| Direction | Inbound |
| Source | My IP Address |
| Destination | Virtual Machine |
| Port | 22 |
| Protocol | TCP |
| Action | Allow |

**Security Best Practice:**  
Allow inbound traffic only from trusted source IP addresses instead of allowing traffic from `Any`.

---

## 2. Outbound Rules

Outbound rules control traffic going **from** an Azure resource to another destination.

For example, an application server may need outbound access to a specific service.

### Example

| Setting | Value |
|---|---|
| Direction | Outbound |
| Source | Application Server |
| Destination | Specific Service |
| Port | 443 |
| Protocol | TCP |
| Action | Allow |

**Security Best Practice:**  
Restrict outbound traffic whenever possible instead of allowing unrestricted Internet access.

---

## 3. Priority

Every NSG rule has a priority number.

The **lower the number, the higher the priority**.

Azure processes NSG rules according to priority, and the first matching rule is applied.

### Example

| Priority | Rule | Action |
|---:|---|---|
| 100 | Allow SSH from Admin IP | Allow |
| 200 | Deny SSH from Internet | Deny |

If traffic matches both rules, priority `100` is processed first, so the traffic is allowed.

### Important

- Lower number = Higher priority
- Higher number = Lower priority
- First matching rule wins
- Custom rules have higher priority than default rules when their priority number is lower

**Recommended practice:** Leave gaps between custom priorities, such as `100`, `200`, `300`, etc., so that new rules can be inserted later.

---

## 4. Source

The **Source** specifies where the traffic is coming from.

A source can be:

- IP Address
- IP Address range
- Virtual Network
- Internet
- Service Tag
- Application Security Group

### Example

```text
Source: 203.0.113.10
