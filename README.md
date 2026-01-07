# Linux EC2 Hardening & Ops Basics on AWS

## Overview

This project demonstrates **secure operation and basic hardening of a Linux EC2 instance** on AWS.  
The focus is on **operational discipline**, **least privilege**, and **safe system administration**, rather than advanced automation.

The instance is accessed **exclusively via AWS Systems Manager (SSM)** — no SSH keys, no inbound ports.

---

## Key Objectives

- Secure access using **SSM Session Manager**
- Eliminate direct root usage
- Apply Linux least-privilege principles
- Inspect services, processes, logs, and filesystem
- Perform safe system hardening
- Validate every change with evidence
- Clean up resources to avoid unnecessary cost

---

## What Was Implemented

- Amazon Linux 2023 EC2 instance
- IAM role with `AmazonSSMManagedInstanceCore`
- Zero inbound security group rules
- Non-root admin user with controlled sudo access
- Service and log inspection using `systemctl` and `journalctl`
- Filesystem and permission validation
- Automatic updates via `dnf-automatic`
- Root login disabled
- Full validation and cleanup documentation

---

## Documentation

- **Build & Ops Guide:** [docs/howto.md](./docs/howto.md)
- **Validation Checklist:** [docs/validation.md](./docs/validation.md)
- **Cleanup Guide:** [docs/cleanup.md](./docs/cleanup.md)
- **Cost Estimate:** [docs/cost-estimate.md](./docs/cost-estimate.md)

---

## Skills Demonstrated

- Linux system administration
- Secure access patterns (SSM over SSH)
- IAM & least privilege
- Service and log management
- Filesystem & permissions
- Responsible system hardening
- Cost-aware cloud operations


