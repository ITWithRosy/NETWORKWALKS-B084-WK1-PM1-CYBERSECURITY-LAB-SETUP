# NETWORKWALKS-B084-WK1-PM1-CYBERSECURITY-LAB-SETUP

## Project Overview

As part of my first week at Networkwalks, I worked on setting up a virtual environment for cybersecurity practice using Oracle VirtualBox and Kali Linux.
The objective was to establish a functional virtual machine and configure its network connectivity.

## Objectives

- Set up Kali Linux as a virtual machine in VirtualBox.
- Create a private VirtualBox NAT Network using the `10.0.0.0/24` IPv4 network.
- Use DHCP for automatic IP address assignment.
- Verify the VM's IP configuration and network connectivity.
- Take a snapshot of the initial configuration of the VM.
- Document the setup and troubleshooting process.
- Prepare the environment for additional virtual machines in later stages.

## Lab Configuration

| Component | Configuration |
|---|---|
| Hypervisor | Oracle VirtualBox |
| Security VM | Kali Linux |
| Virtual network type | NAT Network |
| IPv4 network | `10.0.0.0/24` |
| Address assignment | DHCP |

## Implementation ans results 

1. Importation of kali linux after downloading

2. NAT Network Configuration

The virtual network was created and configured with the IPv4 prefix 10.0.0.0/24,as a NAT Network with DHCP enabled.
[figure1](https://github.com/ITWithRosy/NETWORKWALKS-B084-WK1-PM1-CYBERSECURITY-LAB-SETUP/blob/main/1-Screenshot-%20netwrok-configuration.png)

3. Virtual Machine Setup

Kali Linux was configured as a virtual machine in VirtualBox and connected to the dedicated NAT Network. Plus, a shared folder was created.

4. IP Address and Routing Verification
   
This step was to attribute an IP to the VM manually.

5. Connectivity Testing

The connectivity was tested in order to verify communication with the network gateway and the internet.

6. Snapshot of the VM
The snapshot was to conserve a version of the initial configuration of the VM.

## Troubleshooting

- **Issue:** Internet Connectivity After Static IP Configuration 
- **Diagnosis:** After the manual configuration of the ip address of the VM, the network connection stopped working properly.
- **Resolution:** sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
- **Verification:** The network connection was then restarted and connectivity was tested again.

## Security and Ethical Use

This environment is intended for education and authorized security testing only.

## Tools and Resources

- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- [Kali Linux — Official Download Page](https://www.kali.org/get-kali/)

👤 Author

Ekoum Rosy
Cybersecurity Student 
Linkedin: [https://www.linkedin.com/in/rosy-ekoum](https://www.linkedin.com/in/rosy-ekoum)

📌 Project Information
Program Name: Cybersecurity at Networkwalks | Week: 01 | Project: Cybersecurity & Pentesting Lab Setup | Repository: GitHub
