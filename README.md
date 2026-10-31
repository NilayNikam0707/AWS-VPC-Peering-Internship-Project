# AWS VPC Peering – Internship Project

## Project Overview

This project focuses on establishing communication between two separate Amazon Virtual Private Clouds (VPCs) using AWS VPC Peering.

The setup includes EC2 instances, public and private subnets, route tables, Internet Gateways, and security groups. The main objective was to enable secure communication between private EC2 instances across both VPCs.

## AWS Configuration

**AWS Region:** Asia Pacific (Mumbai) – `ap-south-1`

| Resource | Configuration |
|---|---|
| VPC 1 | Internship-VPC-1 – `10.0.0.0/16` |
| VPC 2 | Internship-VPC-2 – `10.200.0.0/16` |
| VPC1 Public Subnet | `10.0.1.0/24` |
| VPC1 Private Subnet | `10.0.2.0/24` |
| VPC2 Public Subnet | `10.200.1.0/24` |
| VPC2 Private Subnet | `10.200.2.0/24` |
| EC2 Instances | 3 |
| VPC Peering | Active |

## AWS Services Used

- Amazon VPC
- Amazon EC2
- Internet Gateway
- Route Tables
- Security Groups
- VPC Peering Connection

## Implementation

1. Created two custom VPCs with separate CIDR blocks.
2. Configured public and private subnets across both VPCs.
3. Created and attached Internet Gateways.
4. Configured route tables for internet access and communication between VPCs.
5. Established and activated a VPC Peering connection.
6. Launched three EC2 instances across the two VPCs.
7. Configured security group rules to allow the required SSH and ICMP traffic.

## Connectivity Testing

The setup was tested using SSH and ICMP ping commands.

- Connected from the VPC1 public EC2 instance to the VPC1 private EC2 instance.
- Successfully connected from the VPC1 private EC2 instance to the VPC2 private EC2 instance.
- Tested communication between the two private EC2 instances in both directions.

**Result:** Both ping tests were successful, with 4 packets transmitted, 4 received, and 0% packet loss.

## Project Files

- [Project Implementation and Testing Documentation](AWS%20VPC%20Peering%20%E2%80%93%20Project%20Implementation%20and%20Testing.pdf)
- [AWS Project Architecture Diagram](AWS-Project-Architecture.jpeg)

## Learning Outcomes

Through this project, I gained practical experience in AWS networking, VPC configuration, subnetting, route table management, security groups, EC2 deployment, and establishing private communication between VPCs.

---

**Project by:** Nilay N Nikam  
**College:** K.K. Wagh Institute of Engineering Education & Research  
**Course:** B.Tech Information Technology
