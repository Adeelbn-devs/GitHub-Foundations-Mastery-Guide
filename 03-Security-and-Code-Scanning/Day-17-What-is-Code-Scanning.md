# Day 17: What is Code Scanning and CodeQL? 🛡️

**Date:** May 17, 2026  
**Module:** Security and Code Scanning

## 📝 What I Learned Today:

Today, I explored the core mechanics of GitHub's code scanning feature and its native analysis engine, CodeQL.

### 1. The Core Concept
- **Code Scanning:** An automated process that analyzes code to find security vulnerabilities. Alerts are surfaced directly in the repository's **Security tab**.
- **CodeQL:** GitHub’s semantic code analysis engine. It treats "code as data" by creating a database of your codebase and running specialized queries against it to find flaws.

### 2. Three Ways to Setup CodeQL
1. **Default Setup:** The quickest method. GitHub automatically handles the language detection, query suites, and trigger events (runs as a managed GitHub Action without a visible workflow file).
2. **Advanced Setup:** Generates a customizable `.yml` workflow file directly in your repository for fine-tuned control over the scanning process.
3. **External CI:** Run the CodeQL CLI on a third-party CI system (like Jenkins) and upload the results back to GitHub.

### 3. Billing & Actions Minutes
Since native CodeQL scanning uses GitHub Actions:
- **Public Repos:** 100% Free.
- **Private Repos:** Consumes the account's allocated GitHub Actions minutes (e.g., 2,000 minutes for Free accounts).

*Next up: Integrating Third-Party Security Tools!*
