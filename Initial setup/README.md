# SIEMLab — Home Detection Engineering Lab

This folder documents a self-built SOC/detection engineering lab, modeled after [Chris Long's DetectionLab](https://github.com/clong/detectionlab), consisting of an Active Directory Domain Controller, a Windows 10 client, and a Splunk SIEM server deployed via Docker. It demonstrates practical skills in AD and DNS architecture design, network segmentation, Sysmon telemetry forwarding, Splunk Deployment Server management, and preparation for adversary simulation (Atomic Red Team) and memory forensics (Volatility 3). Together, the two documents below show my ability to design, build, and troubleshoot a working SOC environment end-to-end — not just describe one.

## **Architecture & Setup Report**
Covers the design rationale behind the lab: why a hybrid VMware + Docker approach was chosen, the overall network topology, the Gateway vs. DNS distinction, the Client → DC → Forwarder DNS resolution model, resource allocation under a 16 GB RAM constraint, the full deployment sequence, and key lessons learned — including Splunk Deployment Server discipline and Windows-specific DNS quirks.

## **Commands & Configuration Reference**
A consolidated reference of every command and configuration file used to build the lab, organized by host: VMware network setup, PowerShell commands for the Domain Controller and Windows 10 client (AD promotion, DNS forwarder, Sysmon install, Splunk Universal Forwarder setup), and Netplan/bash configuration for the Ubuntu Docker host.
