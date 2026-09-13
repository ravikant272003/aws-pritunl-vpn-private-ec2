# AWS Pritunl VPN – Private EC2 Access

## Overview

Hands-on AWS Cloud & Networking implementation using **Pritunl and OpenVPN** to securely access an EC2 instance in a private subnet without a Public IP.

## Architecture

Windows Client  
↓  
OpenVPN Tunnel  
↓  
Pritunl VPN Server  
↓  
AWS VPC Routing  
↓  
Private Subnet  
↓  
Private EC2

## AWS Configuration

- VPC: `10.0.0.0/20`
- Public Subnet: `10.0.0.0/24`
- Private Subnet: `10.0.1.0/24`
- VPN Network: `10.250.140.0/22`
- VPN: OpenVPN / UDP `14635`
- Private EC2: `10.0.1.135`
- Private EC2 has **No Public IP**

## What I Practiced

- AWS VPC & Subnetting
- Route Tables
- Security Groups
- Pritunl & OpenVPN
- Linux & SSH
- Private EC2 connectivity
- DNS & Let's Encrypt SSL

## Verification

Successfully connected a Windows client to the VPN and accessed the private EC2 instance using SSH.

## Cost Management

AWS resources were terminated after testing to avoid unnecessary cloud charges.

> This repository documents a hands-on learning exercise performed in an AWS environment.
