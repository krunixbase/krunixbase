# Security Policy

## Supported Versions

Use this section to tell people about which versions of your project are
currently being supported with security updates.

| Version | Supported          |
| ------- | ------------------ |
| 5.1.x   | :white_check_mark: |
| 5.0.x   | :x:                |
| 4.0.x   | :white_check_mark: |
| < 4.0   | :x:                |

## Reporting a Vulnerability

Use this section to tell people how to report a vulnerability.

Tell them where to go, how often they can expect to get an update on a
reported vulnerability, what to expect if the vulnerability is accepted or
declined, etc.

## Operational Resilience

This repository enforces modular CI configuration and audit-grade defensibility.

Recent fix: A critical YAML misconfiguration in `.github/dependabot.yml` was identified and resolved. Multiple top-level `updates:` blocks were merged into a single list to restore multi-ecosystem support (pip, GitHub Actions, etc.). This change ensures full CI coverage and prevents silent failures in dependency tracking.

All CI configurations are now linted, deterministic, and version-controlled.

## AI-assisted validation is used to support cryptographic analysis, compliance workflows, and documentation generation.  

All LLM interactions follow reproducible, auditable workflows aligned with the repository’s security model.
