# Cleanup Guide

This guide removes all AWS resources created for this project to avoid unnecessary charges.

---

## Cleanup Steps

1. Exit SSM session
2. Terminate EC2 instance
3. Delete IAM role used for SSM access
4. Remove custom security group (if created)
5. Verify no running EC2 instances or allocated IPs
6. Confirm zero EC2 cost in Billing dashboard

---

## Cleanup Verification

- No EC2 instances running
- No Elastic IPs allocated
- No unused IAM roles
- No active SSM sessions

Cleanup completed successfully.

