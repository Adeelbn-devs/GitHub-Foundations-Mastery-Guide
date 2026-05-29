# Day 25: Set Up, Configure, and Troubleshoot GitHub Copilot ⚙️

**Date:** May 29, 2026  
**Module:** GitHub Copilot

## 📝 What I Learned Today:

Today, I focused on the practical configuration and troubleshooting of the GitHub Copilot extension within Visual Studio Code (VS Code). 

### 1. Installation & Configuration
- **Installation:** Installed directly from the VS Code Extension Marketplace. Requires GitHub account authorization.
- **Enable/Disable:** The status bar icon at the bottom of VS Code allows for a quick global toggle.
- **Language-Specific Rules:** Copilot can be disabled for specific languages (e.g., turning off code completion for `.md` or `.txt` files) to prevent unwanted suggestions during plain text writing. Settings can be accessed via `Preferences > Settings > Extensions > GitHub Copilot`.

### 2. Troubleshooting Connection Issues
When Copilot fails to connect (often due to corporate firewalls, VPNs, or network restrictions), I learned how to debug:
- **Extension Logs:** Accessed via the Command Palette (`Ctrl + Shift + P`) by typing `Developer: Open Extensions Logs Folder`.
- **Electron Logs:** For deeper UI issues, toggling Developer Tools (`Help > Toggle Developer Tools`) reveals Electron-level logs.
- **Collect Diagnostics:** To share issues with GitHub Support, using the command `GitHub Copilot: Collect Diagnostics` generates a comprehensive report of the network and extension state.

*Next up: Getting hands-on with AI-powered code suggestions in the practical exercise!*
