# Networking Basics document for AWS

This document provides a clear overview of essential networking and security concepts used in AWS and modern cloud infrastructures, including public and private subnets, security groups, DNS record types, and SSH key pairs.
---
## 1. Public Subnet
A **public subnet** is a subnet within a Virtual Private Cloud (VPC) that has a direct route to the internet through an **Internet Gateway (IGW)**.  
Resources launched here can receive public IP addresses and are accessible from the internet.

**Common use cases:**
- Web servers  
- Load balancers  
- Bastion hosts  

---
## 2. Private Subnet
A **private subnet** does not have direct internet access.  
Instances inside a private subnet can reach the internet **only through a NAT Gateway or NAT Instance**, while inbound traffic from the internet is blocked.
(Instances here **cannot** be reached directly from the internet. They can still go online but **only through a NAT Gateway**, usually for updates or downloads.)

**Common use cases:**
- Databases  
- Internal services  
- Application backends  
- Sensitive workloads  

---
## 3. Security Groups
A **security group** acts as a virtual firewall for EC2 instances, controlling inbound and outbound traffic at the instance level.

**Key characteristics:**
- **Stateful:** return traffic is automatically allowed (if an incoming connection is allowed, the reply is also allowed automatically)
- **Allow rules only:** no explicit deny rules (They can only **allow** traffic, not block it )
- **Instance-level protection** rather than subnet-level (They protect your instance, not the whole subnet)

**Examples:**
- Allow SSH (port 22) from your IP  
- Allow HTTP (80)
- HTTPS (443) for web servers  

---
## 4. DNS Record Types Supported by Route 53

| Record Type | Purpose |
|-------------|---------|
| **A** | Maps a domain to an IPv4 address |
| **AAAA** | Maps a domain to an IPv6 address |
| **CNAME** | Points one domain to another domain name |
| **MX** | Identifies mail servers for email delivery |
| **TXT** | Used for verification or security policies (e.g., SPF) |
| **NS** | Specifies the authoritative name servers for a domain |
| **SRV** | Defines service locations (e.g., SIP, XMPP) |
| **PTR** | Reverse DNS lookup (IP → domain) |
| **SOA** | Contains domain-level administrative information |
| **CAA** | Specifies which Certificate Authorities can issue certificates |
| **Alias** | Route 53-specific record that maps to AWS resources (ELB, CloudFront, S3) |

---
## 5. How SSH Key Pairs Work

SSH key pairs provide secure, password-less authentication when connecting to Linux servers such as EC2 instances.
### Components
- **Public key:** Stored on the server  
- **Private key:** Stored securely on your machine

### How it works
1. You initiate an SSH connection using your private key.  
2. The server checks whether the corresponding public key exists in `~/.ssh/authorized_keys`.  
3. If the keys match, access is granted without sending passwords over the network.  

### Why it is secure
- Uses asymmetric cryptography  
- Private key never leaves your machine  
- Prevents brute-force password attacks

---
This file provides the foundational networking concepts needed for DevOps beginners and cloud engineers working with AWS.
