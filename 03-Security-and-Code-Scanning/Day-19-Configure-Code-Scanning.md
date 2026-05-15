# Day 19: Configure Code Scanning ⚙️🛡️

**Date:** May 19, 2026  
**Module:** Security and Code Scanning

## 📝 What I Learned Today:

Today, I explored how to customize CodeQL analysis by switching from Default to **Advanced Setup**. This generates a `codeql-analysis.yml` workflow file, giving administrators granular control over when and how code scans run.

### 1. Workflow Triggers (Frequency)
You can configure code scanning to run on specific events:
- **`on: push`**: Scans every push to default/protected branches. Results show in the Security tab.
- **`on: pull_request`**: Scans PRs targeting the default branch. It specifically scans the *merge commit* for more accurate results and surfaces alerts directly in the PR checks.
- **`on: schedule`**: Uses `cron` syntax to run periodic scans (e.g., weekly). Crucial for catching newly discovered zero-day vulnerabilities in older, unmaintained code.

### 2. Pull Request Check Failures
By default, a PR check will **fail** (blocking the merge) if CodeQL detects an alert with a severity level of **Error**, **Critical**, or **High**. Admins can modify these thresholds in the repository's `Code security and analysis` settings.

### 3. Cost & Time Optimization
To prevent wasting GitHub Actions minutes on irrelevant changes (like documentation updates), you can use the `paths-ignore` array in your workflow:

```yaml
on:
   pull_request:
      branches: [main]
      paths-ignore:
         - '**/*.md'
         - '**/*.txt'
