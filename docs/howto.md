# Build & Operations Guide

This document outlines the step-by-step implementation of the Linux EC2 Hardening & Ops project.

---

## Phase 1 — Secure EC2 Access via SSM

- Launched Amazon Linux 2023 EC2 instance
- No SSH key pair created
- No inbound security group rules
- IAM role attached with `AmazonSSMManagedInstanceCore`
- Connected using SSM Session Manager

[Phase 1 Screenshots](https://github.com/vikasreddy98/AWS-project-linux-ec2-hardening-and-ops/tree/afc15a7d569e06d3a8f8db04d3094db2881f0249/screenshots/Phase%201)

---

## Phase 2 — Users, Groups & Least Privilege

- Identified execution context (`whoami`, `id`)
- Created non-root admin user (`opsadmin`)
- Configured group-based sudo access
- Verified controlled privilege escalation
- Locked unused default user access

[Phase 2 Screenshots](https://github.com/vikasreddy98/AWS-project-linux-ec2-hardening-and-ops/tree/7700012f225fc5b9084cc04aa2067bf27095e05f/screenshots/Phase%202)


---

## Phase 3 — Services, Processes & Logs

- Inspected running processes (`ps`, `top`)
- Managed system services using `systemctl`
- Restarted and validated SSM agent
- Inspected logs using `journalctl`
- Verified outbound network connectivity

[Phase 3 Screenshots](https://github.com/vikasreddy98/AWS-project-linux-ec2-hardening-and-ops/tree/7700012f225fc5b9084cc04aa2067bf27095e05f/screenshots/Phase%203)

---

## Phase 4 — Filesystem & Permissions

- Explored Linux directory structure
- Located and inspected system logs
- Applied ownership and permission changes
- Verified permission enforcement
- Checked disk usage

[Phase 4 Screenshots](https://github.com/vikasreddy98/AWS-project-linux-ec2-hardening-and-ops/tree/7700012f225fc5b9084cc04aa2067bf27095e05f/screenshots/Phase%204)

---

## Phase 5 — Basic Hardening

- Installed and enabled automatic updates (`dnf-automatic`)
- Reviewed unused packages safely
- Verified firewall and listening ports
- Confirmed root password login disabled
- Validated post-hardening access

[Phase 5 Screenshots](https://github.com/vikasreddy98/AWS-project-linux-ec2-hardening-and-ops/tree/7700012f225fc5b9084cc04aa2067bf27095e05f/screenshots/Phase%205)


