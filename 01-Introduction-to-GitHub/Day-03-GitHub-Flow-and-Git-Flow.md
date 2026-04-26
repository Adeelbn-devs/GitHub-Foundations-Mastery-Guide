# Day 3: Components of the GitHub Flow 🚀

**Date:** April 27, 2026  
**Module:** Introduction to GitHub

## 📝 What I Learned Today:

Today's focus was on the core mechanisms of version control and team collaboration. Understanding how code moves from a local machine to production is critical.

### 1. The Core Components
- **Branches:** A safe, isolated workspace. You branch off the `main` line to experiment or build features without risking the production code.
- **Commits:** A snapshot of your changes. 
  - **File States:** Files move through specific states before being committed: `Untracked` -> `Tracked` (`Unmodified` -> `Modified` -> `Staged`) -> `Committed`.
- **Pull Requests (PRs):** The formal request to merge your branch's commits into the base branch. This is where code reviews, approvals, and discussions happen.

### 2. GitHub Flow vs. Git Flow

| Feature | GitHub Flow | Git Flow |
| :--- | :--- | :--- |
| **Complexity** | Lightweight & Simple | Structured & Heavy |
| **Best For** | Continuous Delivery (Web apps) | Versioned Releases (Enterprise/Software) |
| **Default Branch** | `main` | `master` and `develop` |
| **Process** | Branch -> Commit -> PR -> Merge | Uses specialized branches (`feature`, `release`, `hotfix`) |

### 3. The Git Flow Branching Model
If using the strict Git Flow, these branches dictate the lifecycle:
- `master`: Always production-ready.
- `develop`: The integration branch for the next release.
- `feature/*`: Branched from `develop` for new work.
- `release/*`: Prepares a new production release (testing/bug fixes).
- `hotfix/*`: Emergency patches directly off `master`.

*Next up: Mastering GitHub as a Collaborative Platform (Issues & Discussions)!*
