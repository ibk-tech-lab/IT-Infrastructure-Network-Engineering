# Lab 01: VirtualBox and Ubuntu Server Installation

## Status

**Completed and visually verified:** VirtualBox VM setup, Ubuntu Server boot/login, Ubuntu release, and NAT network interface.  
**Evidence:** Screenshots supplied and reviewed during the learning session. Repository image files are still to be added.

## Objective

Set up a virtualised Linux server environment on a Windows computer so that I can practise Ubuntu Server administration without replacing my main operating system.

## Environment and Tools

- Host operating system: Windows 11
- Computer memory: 16 GB RAM
- Processor: Intel Core i5
- Virtualisation software: Oracle VirtualBox
- Guest operating system: Ubuntu Server 26.04.1 LTS

## Work Completed

- Installed Oracle VirtualBox.
- Created and started an Ubuntu Server virtual machine.
- Reached the Ubuntu terminal and logged in successfully.
- Ran the Ubuntu release and network-interface checks.
- Captured screenshots of the VM overview and terminal output.

## Verified Virtual Machine Configuration

| Item | Verified value |
|---|---|
| Virtual machine name | Ubuntu Server 26.04 |
| Guest OS release | Ubuntu 26.04.1 LTS |
| Codename | Resolute |
| Allocated memory (RAM) | 4096 MB (4 GB) |
| Allocated processors | 2 |
| Virtual disk | 30.00 GB, VDI |
| Network attachment mode | NAT |
| Network interface | enp0s3 |
| IPv4 address | 10.0.2.15 (private NAT address) |
| Login / terminal access | Successful |

The screenshots show the VM powered on and later powered off. The terminal shows a successful shell prompt and output from `lsb_release -a` and `ip addr`.

## Commands Practised

Ubuntu release information:

```bash
lsb_release -a
```

Network interface information:

```bash
ip addr
```

The release command reports:

- Distributor ID: Ubuntu
- Description: Ubuntu 26.04.1 LTS
- Release: 26.04
- Codename: resolute

The network output shows the `enp0s3` interface in the UP state with IPv4 address `10.0.2.15/24`. This is consistent with a VirtualBox NAT network.

## Configuration Note

The VirtualBox overview identifies the guest operating-system profile as **Ubuntu 25.04 (Plucky Puffin) 64-bit**, while the installed guest reports **Ubuntu 26.04.1 LTS**. This is a VirtualBox profile-label mismatch, not evidence that the Ubuntu installation itself is incorrect. Review the VM's General settings and select the closest available Ubuntu 64-bit profile if VirtualBox offers a matching release.

## Update / Maintenance Observation

One terminal screenshot shows package configuration and service-restart messages, followed by a shell prompt. This indicates that package setup activity took place. A fresh `sudo apt update` and `sudo apt upgrade` should still be run and verified as part of the initial maintenance checklist.

## Screenshots

The supplied evidence reviewed includes:

- VirtualBox VM overview showing memory, processors, disk, and NAT.
- Ubuntu Server terminal after package configuration.
- Ubuntu release information.
- Network interface and IPv4 address.
- VirtualBox Manager home screen.

The image files themselves still need to be committed to this repository under the `Screenshots/` directory.

## Challenges and Troubleshooting

- The command was initially entered as `lsb release -a`, which produced a command-not-found message. It was then corrected to `lsb_release -a`, which returned the Ubuntu release information successfully.
- The VirtualBox guest OS profile label differs from the installed Ubuntu release. Review the profile setting as noted above.

## What I Learned

- VirtualBox allows Ubuntu Server to run as a guest operating system inside a Windows host.
- The VM is configured with 4 GB RAM, 2 virtual processors, and a 30 GB virtual disk.
- The NAT network provides the guest with a private IPv4 address.
- `lsb_release -a` identifies the installed Ubuntu release.
- `ip addr` displays network interfaces, their state, and assigned IP addresses.

## Next Steps

1. Review the VirtualBox guest OS profile label.
2. Run `sudo apt update` and `sudo apt upgrade`, then verify the result.
3. Test connectivity with `ping -c 4 1.1.1.1` and `ping -c 4 ubuntu.com`.
4. Check disk and memory usage with `df -h` and `free -h`.
5. Confirm whether OpenSSH Server is installed and active.
6. Begin the first Linux command-line and system administration exercises.

---

*Configuration values in this log are based on the supplied screenshots. Items not shown in the screenshots are not marked as verified.*
