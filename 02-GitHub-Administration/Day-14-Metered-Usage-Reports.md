# Day 14: Metered Usage Reports 📊

**Date:** May 14, 2026  
**Module:** Introduction to GitHub Administration

## 📝 What I Learned Today:

Today, I explored how to monitor and optimize GitHub’s metered products. Understanding these consumption metrics is crucial for preventing budget overruns.

### 1. GitHub Actions Minutes
- **Usage:** Billed based on OS runner type (Linux is cheapest, macOS is the most expensive) and execution minutes.
- **Optimization:** Use self-hosted runners for heavy workflows and cache dependencies.

### 2. GitHub Packages
- **Usage:** Metered based on storage (GB) and data transfer (bandwidth).
- **Optimization:** Regularly delete unused artifacts/images.

### 3. GitHub Enterprise (GHE) Licenses
- **Usage:** Billed per active user with access to private repositories.
- **Optimization:** Audit inactive users and automate provisioning with SSO/SCIM.

### 4. GitHub Advanced Security (GHAS)
- **Usage:** Billed per **Unique Active Committer** (anyone who has pushed a commit to a GHAS-enabled repo in the last **90 days**).
- **Optimization:** Only enable GHAS on repositories that strictly require advanced security scanning.

### 5. GitHub Copilot
- **Usage:** Billed per user (Free for students and verified open-source maintainers).
- **Optimization:** Deactivate licenses for users not utilizing the AI features.

### 6. Git Large File Storage (LFS)
- **Usage:** Billed for storing large binary files (1GB free storage/bandwidth per account).
- **Optimization:** Prune unreferenced objects or offload massive binaries to external blob storage like AWS S3.

*Next up: Module Assessment!*
