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

## Issue Faced 
During my Kali Linux lab setup, I faced a network connectivity issue."

## Issue Fixed by Code 
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0

## Comment on Issue Faced and Fixed

This helped and connectivity was restored and I verified connectivity using ping commands (Ping 8.8.8.8 and Ping Google.com) and i aslo went on google to show that the connection is fine. I checked the network settings using nmcli and applied the fix:



