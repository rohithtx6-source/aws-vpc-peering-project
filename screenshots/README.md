AWS VPC Peering Project

Project Overview

This project demonstrates how to establish private network connectivity between two Amazon Virtual Private Clouds (VPCs) using AWS VPC Peering.

AWS Services Used

* Amazon VPC
* Amazon EC2
* VPC Peering
* Subnets
* Route Tables
* Internet Gateway
* Security Groups

Network Configuration

VPC A

* CIDR: 10.10.0.0/16
* Public subnet: 10.10.1.0/24
* Private subnet: 10.10.2.0/24

VPC B

* CIDR: 10.20.0.0/16
* Private subnet: 10.20.1.0/24

Implementation Steps

1. Created two VPCs with separate CIDR blocks.
2. Created public and private subnets.
3. Attached an Internet Gateway to VPC A.
4. Launched a bastion host and two private EC2 instances.
5. Created and accepted a VPC Peering connection.
6. Configured route tables and security groups.
7. Connected to the private instances using SSH through the bastion host.
8. Tested connectivity between the private instances using ping.

Connectivity Test

Successfully tested connectivity in both directions between the private instances.

* VPC A private instance: 10.10.2.202
* VPC B private instance: 10.20.1.170
* Result: 4 packets received, 0% packet loss.

Outcome

Verified private network communication between two VPCs using VPC Peering.

Author

Rohith Thommandru
