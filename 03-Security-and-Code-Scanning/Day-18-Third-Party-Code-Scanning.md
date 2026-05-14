# Day 18: Enable Code Scanning with Third-Party Tools 🛡️

**Date:** May 18, 2026  
**Module:** Security and Code Scanning

## 📝 What I Learned Today:

Today, I learned how to integrate external, third-party security tools (like ESLint or Snyk) with GitHub Advanced Security. GitHub doesn't force you to use CodeQL; you can bring your own scanner!

### 1. The Magic Format: SARIF
- To display third-party alerts in GitHub's Security tab, the external tool must output results in **SARIF version 2.1.0** (Static Analysis Results Interchange Format).

### 2. How to Upload SARIF Files
There are three main methods to upload these results to GitHub:
1. **GitHub Actions:** Use the native `github/codeql-action/upload-sarif` action. You just provide the `sarif_file` path.
2. **REST API:** Use the `/analyses` endpoint with the custom media type `application/sarif+json`.
3. **CodeQL CLI:** Used when running analysis on external CI/CD systems (like Jenkins) or local machines.

### 3. Key Constraints & Concepts (Exam Focus)
- **Preventing Duplicates:** GitHub uses the `partialFingerprints` property in the SARIF file to track bugs and prevent showing duplicate alerts across multiple scans.
- **Result Limits:** A maximum of **5,000 results** per upload is supported.
- **Size Limits:** The SARIF file cannot exceed **10 MB** (gzip-compressed).

*Next up: Learning how to configure and trigger these scans!*
