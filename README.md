# Vulnerabilities Tracking

This repository automates the identification and tracking of security vulnerabilities across the projects defined in repositories.json. By utilizing govulncheck, it continuously monitors targeted codebases and their dependencies to ensure a robust security posture.

Findings are automatically converted into GitHub Issues, providing a structured workspace for triage, documentation, and resolution of discovered vulnerabilities.

## How it Works

1. **Source Configuration**: The repositories.json file contains a list of Go-based repositories to be monitored.
2. **Scanner**: Govulncheck is used to analyze these repositories for known vulnerabilities in their dependency trees.
3. **Issue Creation**: For every new vulnerability detected that isn't already tracked, an issue is automatically opened in this repository containing the scan report and affected versions.
