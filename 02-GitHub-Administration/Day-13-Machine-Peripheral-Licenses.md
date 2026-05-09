# Day 13: License Usage Stats in Machine and Peripheral Devices 🤖

**Date:** May 13, 2026  
**Module:** Introduction to GitHub Administration

## 📝 What I Learned Today:

Today, I explored how automation impacts enterprise billing. Human developers aren't the only ones consuming GitHub licenses; automation bots and external integrations do too!

### 1. Machine Accounts
- **Definition:** GitHub accounts used purely for automation, scripts, or third-party tools.
- **The Catch:** Each machine account acts independently and **consumes a full GitHub license**, exactly like a human user.
- **Tracking:** Admins can find inactive machine accounts via the `Enterprise Admin Console` or by using the `GraphQL API` to check their `lastActiveAt` timestamp.

### 2. Peripheral Services
- **Definition:** External integrations and CI/CD tools that interact with GitHub via API requests (e.g., Jenkins, GitHub Actions Runners, Dependabot, Slack).
- **Tracking:** Tracked via `REST API` and Audit Logs to detect idle self-hosted runners or inactive integrations wasting resources.

### 3. Best Practices for Admins
- **Audit Regularly:** Identify and deactivate stale machine accounts to free up expensive licenses.
- **Restrict Permissions:** Enforce the principle of least privilege. A compromised machine account with admin access is a massive security risk.
- **Optimize Runners:** Shut down idle self-hosted runners to reduce infrastructure and API costs.

*Understanding this is crucial for balancing robust CI/CD automation with strict cost control and security compliance.*
