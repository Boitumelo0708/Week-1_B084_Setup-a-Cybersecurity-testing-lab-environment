# Week-1_B084_Setup-a-Cybersecurity-testing-lab-environment
Cybersecurity Lab Setup

# Week 1 - Security Testing Lab Environment Setup

## Overview
Set up a personal cybersecurity lab using VirtualBox and Kali Linux in an isolated NAT Network environment.

**Lab Details:**
- Hypervisor: Oracle VirtualBox
- OS: Kali Linux (OVA Import)
- Network: NATNetwork - 10.0.0.0/24
- VM IP: 10.0.0.2

## Steps Completed
1. Downloaded VirtualBox, Extension Pack and Kali Linux VirtualBox image
2. Installed VirtualBox
3. Created NAT Network (10.0.0.0/24) with DHCP enabled
4. Imported Kali Linux into VirtualBox
5. Configured VM settings: Network to NATNetwork, Clipboard Bidirectional, Drag & Drop Bidirectional, Shared Folder (Downloads)
6. Configured IP settings and verified internet access

<img width="1780" height="1217" alt="Machine Snapshot" src="https://github.com/user-attachments/assets/3a7fcf8e-c1c5-443b-b7d7-62268da69a31" />

## Issue Faced 
During my Kali Linux lab setup, I faced a network connectivity issue."

## Issue Fixed by Code 
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0

## Comment on Issue Faced and Fixed

This helped and connectivity was restored and I verified connectivity using ping commands (Ping 8.8.8.8 and Ping Google.com) and i aslo went on google to show that the connection is fine. I checked the network settings using nmcli and applied the fix:

<img width="1531" height="1055" alt="Kali Linux Wired Connection" src="https://github.com/user-attachments/assets/7b2a2e4e-599e-4a69-b308-d1d25a8b5af2" />



