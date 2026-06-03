# linux-homelab
This repository documents my journey learning Linux system administration, networking, Docker, and self-hosted infrastructure.

## Goals

- Learn Ubuntu Server
- Learn terminal workflows
- Learn Docker and containers
- Learn networking and security
- Host multiplayer game servers
- Implement cloud storage solution
- Improve Git and GitHub workflows
- Learn industry-standard development practices
- Practice infrastructure documentation

## Current Hardware

- Dell OptiPlex 3040 Micro
- MacBook Pro
- Linux Mint desktop
- Steam Deck for additional testing

## Current Progress

- Hosting Valheim server (Desktop)
- Hosting Core Keeper server (Desktop)
- Learning Linux terminal basics
- Researching Ubuntu Server and Proxmox

## Planned Technologies

- Ubuntu Server
- Docker
- Tailscale
- Proxmox
- UFW Firewall
- Nginx

## Day 1 - Ubuntu Server

### Objectives

- Install Ubuntu Server on Dell OptiPlex 3040 Micro
- Configure networking
- Enable remote administration

### Completed

- Created bootable Ubuntu Server using balenaEtcher
- Successfully installed Ubuntu Server
- Configured networking with DHCP
- Troubleshot minor networking issues
- Installed and enabled OpenSSH server
- First remote connection established using Linux Mint Desktop
- Verified remote admin works
- Verified server survives reboot and remains accessible
- Configured SSH key authentication between Linux desktop and homelab server
- Generated and registered SSH key for server-to-GitHub authentication
- Verified passwordless SSH access
- Verified GitHub SSH authentication from the server 

### Lessons learned

- Difference between a phone cable and ethernet (It was late)
- How Ubuntu detects network interfaces
- How DHCP assigns IP addresses
- Importance of verifying physical connectivitiy before
  troubleshooting software
- Using SSH to establish trust between machines
- How GitHub uses SSH keys for repository access

### Next Steps

- DHCP reservation
- Install Tailscale
- Migrate gameservers from desktop to server

