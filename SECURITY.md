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

## AI Security Model

The Krunixbase ecosystem incorporates AI‑assisted components strictly within a controlled, auditable, and security‑aligned framework. AI/LLM functionality is designed to support cryptographic analysis, compliance workflows, and documentation generation without introducing new attack surfaces or weakening cryptographic guarantees.

Isolation and Trust Boundaries

- AI components operate in a sandboxed environment fully isolated from cryptographic primitives, secret‑handling logic, and threshold reconstruction workflows.

- No secret material, key fragments, or sensitive cryptographic artifacts are ever exposed to AI systems.

- LLMs do not participate in cryptographic decision‑making and cannot override deterministic validation results.

Deterministic and Auditable Workflows

- All LLM interactions follow fixed, versioned, and reproducible prompt templates.

- Outputs are deterministic within the constraints of the model and are validated against cryptographic truth before being accepted into any workflow.

- Every AI‑assisted operation generates a traceable audit log entry aligned with the repository’s security and compliance model.

Data Handling and Privacy Guarantees

- No user data, evidence, or cryptographic material is used for model training.

- All inference is stateless and ephemeral.

- AI components process only metadata, structural information, and non‑sensitive representations of evidence.

Operational Constraints

- AI systems serve as analytical and documentation‑support components, not autonomous decision engines.

- AI‑generated outputs are advisory and must pass deterministic validation layers before integration into forensic or compliance artifacts.

- The system enforces strict separation between AI‑assisted analysis and authoritative cryptographic verification.

Risk Mitigation

- AI components cannot modify evidence, cryptographic artifacts, or validation results.

- All outputs are subject to human or deterministic review in workflows requiring audit‑grade assurance.

- The architecture prevents model hallucinations from influencing cryptographic or compliance outcomes.
