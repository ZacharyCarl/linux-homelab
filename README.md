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

## Planned Technologies

- Ubuntu Server
- Docker
- Tailscale
- Proxmox
- UFW Firewall
- Nginx


# Current Progress

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
- Configured SSH key authentication between MacBook and homelab server
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

## Day 2 - Docker Fundamentals and Server Migration

### Objectives

- Develop a fundamental understanding of Docker and learn basic commands
- Successfully migrate an existing Core Keeper server from my Linux desktop to the homelab

### Completed

- Completed introductory Docker exercises and established a foundational understanding of Docker concepts
- Successfully transferred the Core Keeper server and save data using `scp`
- Created a systemd service file and configured the server to start automatically on boot

### Lessons Learned

- Basic Docker architecture: Image → Container → Volume
- The difference between persistent and disposable components in Docker
- Fundamentals of Docker port mapping
- How to use `scp` to securely copy files between Linux systems
- First experience writing a YAML file and using Docker Compose
- Basic service management with `systemd` and `systemctl`

### Next Steps

- Understand and begin working with Docker volumes and bind mounts
- Containerize the Core Keeper server
- Migrate and containerize the Valheim server
- Use Docker Compose to manage and launch game servers
- Configure Tailscale for secure remote access

## Day 3 - Migrating to Proxmox after brief hiatus

### Undocumented Changes

- Created Valheim and Palworld servers using steamcmd
- Created systemd service files

### Objectives

- Back up existing Ubuntu Server
- Verify backup integrity
- Copy backup archive to another machine
- Create bootable Proxmox USB
- Install Proxmox VE
- Configure networking
- Verify SSH and web interface access
- Create Ubuntu Server VM
- Update and install required packages
- Restore SSH keys
- Restore game server files and configuration
- Restore systemd service files
- Verify servers start successfully
- Verify server savestates and integrity
- Confirm external connectivity
- Create first promox snapshot

### Completed

- Successfully backed up Ubuntu Server using 'tar'
- Transfered backup to Mac using 'sftp'
- Successfully installed Proxmox VE
- Successfully configured networking
- Confirmed browser access
- Switched from enterprise repository to no subscription
- Successfully deployed Ubuntu Server VM
