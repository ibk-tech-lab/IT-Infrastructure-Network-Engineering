# Lab 01: VirtualBox and Ubuntu Server Installation

## Status

**Completed:** Initial software installation, as reported during the learning session.  
**Evidence:** Screenshots are pending review and upload.

## Objective

Set up a virtualised Linux server environment on a Windows computer so that I can practise Ubuntu Server administration without replacing my main operating system.

## Environment and Tools

- Host operating system: Windows 11
- Computer memory: 16 GB RAM
- Processor: Intel Core i5
- Virtualisation software: Oracle VirtualBox
- Guest operating system: Ubuntu Server

## Work Completed

- Installed Oracle VirtualBox.
- Installed Ubuntu Server for the practical learning environment.

## Configuration Record

The exact virtual machine configuration has not yet been recorded. The following details will be confirmed from the VirtualBox settings and Ubuntu system information:

| Item | Recorded value |
|---|---|
| Ubuntu Server release | To be confirmed |
| Virtual machine name | To be confirmed |
| Allocated memory (RAM) | To be confirmed |
| Allocated processors | To be confirmed |
| Virtual disk size | To be confirmed |
| Network attachment mode | To be confirmed |
| OpenSSH installation/status | To be confirmed |

## Verification To Do

The next step is to verify that Ubuntu boots correctly and collect basic system information. After logging in to the Ubuntu Server terminal, run:

```bash
lsb_release -a
```

```bash
hostnamectl
```

```bash
ip addr
```

```bash
free -h
```

```bash
df -h
```

Record the outputs (excluding sensitive information) and add screenshots as evidence.

## Screenshots

Screenshots will be added here after review:

- VirtualBox application / VM list
- Ubuntu VM configuration (memory, CPU, storage)
- Ubuntu Server installation or login screen
- Ubuntu terminal showing successful login
- Ubuntu version and system information

## Challenges and Troubleshooting

No installation problems have been documented yet. Any errors or fixes encountered during verification will be recorded here.

## What I Learned

This setup introduces the concept of virtualisation: VirtualBox runs Ubuntu Server as a guest operating system inside the Windows host. This provides an isolated practice environment for learning server administration.

## Next Steps

1. Confirm Ubuntu Server starts and accepts login.
2. Record the Ubuntu release and VM hardware settings.
3. Verify network connectivity.
4. Update package lists and apply available system updates.
5. Begin the first Linux command-line and system administration exercises.

---

*This log records only the installation work reported so far. Configuration values, test results, and screenshots will be added after they have been checked.*
