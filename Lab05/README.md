# CSA15 GP-VM-01 – Guided VM/IaaS Lab

## Student Details

- Name: VARSHINI
- Course/Lab: CSA15
- Experiment: GP-VM-01 Guided VM/IaaS Experiment

## Environment

| Item | Configuration |
|---|---|
| Host OS | Windows |
| Hypervisor | Oracle VirtualBox |
| VirtualBox Version | 7.2.14 r174565 |
| Guest OS | Ubuntu 26.04 LTS |
| VM Name | csa15-localvm-192472358 |
| CPU | 1 CPU |
| RAM | 2048 MB |
| Virtual Disk | 25 GB VDI |
| Network | NAT |
| Guest Username | student |

## Configuration Decisions

An existing Ubuntu 26.04 LTS virtual machine was reused instead of creating a new VM. This reduced the need for an additional OS download and avoided unnecessary storage consumption on the host.

The VM was configured with 1 CPU and 2048 MB RAM. NAT networking was used to provide network connectivity to the guest OS.

The existing virtual disk is 25 GB. It was retained because Ubuntu was already installed and functioning correctly.

## Verification

The guest operating system was verified using:

- `lscpu` – CPU verification
- `free -h` – RAM verification
- `df -h` – storage verification
- `ip addr` – network verification

The guest OS successfully detected 1 CPU, approximately 2 GB assigned memory, available filesystem storage, and an active NAT network interface.

## Screenshot Index

| Screenshot | Evidence |
|---|---|
| 01 | Host CPU and virtualization readiness |
| 02 | Oracle VirtualBox |
| 03 | VM hardware configuration |
| 04 | Ubuntu guest OS boot |
| 05 | CPU verification using lscpu |
| 06 | RAM verification using free -h |
| 07 | Storage verification using df -h |
| 08 | Network verification using ip addr |

## Cleanup Status

The VM was used only for the guided lab activity. No additional VM was created. The existing VM can be powered off after completion to release host CPU and RAM resources.

## Result

The Ubuntu virtual machine was successfully run using Oracle VirtualBox and verified for CPU, RAM, storage, and network availability.
