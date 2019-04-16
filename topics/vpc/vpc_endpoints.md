# VPC Endpoint  

A VPC endpoint enable to you privately connect your VPC to supported AWS services and VPC endpoints services powered by PrivateLink without requiring an internet gateway, NAT device, VPN connection, or AWS Direct Connect. Instances in your VPC do not require public IP addresses to communicate with resources in the service.  

Endpoint are virtual devices. They are horizontally scaled, redundant, and Highly available VPC components that allow communicate between instances in your VPC and services without imposing availability risk or bandwidth constraints on your network traffic.  

Two types of VPC endpoints:
* Interface Endpoints;  

> Is an elastic network interface with a private IP address that serves as an entry point for traffic destined to a supported service.

* Gateway Endpoints;  

Currently Gateway Endpoints Support:

* S3
* DynamoDB

[NEXT - Tips](vpc/tips.md)
