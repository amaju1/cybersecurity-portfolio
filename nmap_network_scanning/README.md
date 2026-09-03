# Nmap Network Scanning Lab

## Objective

To learn how Nmap can be used to discover open ports

and identify services running on an authorized laboratory system.

## Lab Environment

- Operating System: Kali Linux

- Virtualization: VirtualBox

- Target: Personal/authorized cybersecurity lab

- Tool: Nmap

## Methodology

1. Identified the IP address of the laboratory target.

2. Tested connectivity between Kali Linux and the target.

3. Performed a basic Nmap scan.

4. Performed service and version detection using Nmap.

## Commands

nmap <TARGET-IP>

nmap -sV <TARGET-IP>

## Findings

The scan identified several open TCP ports and the services

associated with them.

## What I Learned

- How Nmap performs network reconnaissance.

- How to identify open ports.

- How to identify running services.

- Why exposed services can increase an attack surface.

## Security Considerations

All scanning was performed against an authorized laboratory

environment. Network scanning should only be performed against

systems where permission has been granted.
