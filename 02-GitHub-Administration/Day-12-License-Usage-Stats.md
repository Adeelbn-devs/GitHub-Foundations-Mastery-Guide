# Day 12: License Usage Stats 📊

**Date:** May 12, 2026  
**Module:** Introduction to GitHub Administration

## 📝 What I Learned Today:

Today, I explored how GitHub Enterprise administrators track and optimize seat licenses to manage costs effectively.

### 1. Key Billing Concept: Prepaid vs. PAYG
- **Prepaid:** You buy a set number of seats upfront and can view "Available Licenses."
- **Pay-As-You-Go (PAYG):** The modern default. You are billed purely based on "Active Seats" consumed during the month.

### 2. Methods to Track License Usage
GitHub provides dual approaches (UI and API) to track usage across different structural levels:
- **Single Organization:** Navigate to `Settings > Billing & plans`. (Can also be queried using the GraphQL API).
- **Multiple Organizations (Enterprise Cloud):** Navigate to `Enterprise settings > Billing > License Usage`.
- **GitHub Enterprise Server (GHES):** Monitored via the GHES Admin Console or by hitting the REST API (`/enterprises/YOUR-ENTERPRISE/license`).
- **Multiple GHES Instances:** Tracked via the Enterprise Metrics API.

### 3. Best Practices for License Management
- **Automate Monitoring:** Use REST or GraphQL APIs to programmatically track seat usage.
- **Reclaim Unused Seats:** Identify and remove inactive users to stop paying for unused licenses.
- **Audit Regularly:** Conduct periodic financial reviews to optimize resource allocation.

*Next up: License Usage Stats in Machine and Peripheral Devices!*
