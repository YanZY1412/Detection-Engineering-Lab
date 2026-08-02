# Detection Engineering Lab

This repository documents a self-built home lab used to practice detection engineering, incident investigation, and adversary simulation, along with the case studies built on top of it. It's organized into a base infrastructure setup and a growing set of individual detection cases, each modeled on realistic attack techniques and mapped to MITRE ATT&CK.

## Repository Structure

```
.
├── Initial setup/                  # Base lab infrastructure (AD, Win10, Splunk)
│   ├── README.md
│   ├── 01_SIEMLab-Architecture-and-Setup.md
│   └── 02-Commands-and-Configuration.md
│
└── Webshell-upload-detection/      # Case: T1505.003 – webshell upload detection (upcoming)
    └── ...
```

## Base Lab

The [`Initial setup/`](./Initial setup) folder contains the foundation all subsequent cases are built on: an Active Directory Domain Controller, a domain-joined Windows 10 client, and a Splunk SIEM server (via Docker), with Sysmon forwarding endpoint telemetry for analysis. See its README for the full architecture, network design, and deployment steps.
