## [v2.0-dual-licensing] — 2026-01-10

### 🔐 Licensing & Repository Structure
– Introduced dual licensing model:
  – `docs/` licensed under CC-BY 4.0
  – `src/` licensed under GNU GPL v3.0
– Added dedicated LICENSE files per directory
– Updated root LICENSE with links to sub-licenses
– Clarified licensing boundaries in `LEGAL_INTERPRETATION.md`

### 📁 Modular Layout
– Separated documentation (`docs/`) and source code (`src/`)
– Updated `README.md` to reflect modular structure and licensing
– Added `REFERENCE.md` to codify architectural intent

### 🛡️ Security & Governance
– Created `SECURITY.md` with operational resilience model
– Added `CODE_OF_CONDUCT.md` and `CONTRIBUTING.md` for governance clarity

### ⚙️ CI Hardening
– Refactored `.github/dependabot.yml`:
  – Merged duplicated `updates:` blocks
  – Removed unsupported YAML fields
  – Restored multi-ecosystem support (pip, GitHub Actions)
– Verified deterministic CI behavior and audit-grade compatibility

### 🧾 Documentation & Templates
– Added GitHub issue templates
– Clarified contribution boundaries and review expectations

---

This release marks the transition to a fully modular, defensible, and audit-ready repository architecture.
