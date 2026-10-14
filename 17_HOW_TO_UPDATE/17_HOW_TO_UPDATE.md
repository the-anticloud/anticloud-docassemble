# How to Update — DOCASSEMBLE

**Project:** `DOCASSEMBLE`
**Category:** LEGAL_TECH
**Domain:** legal technology
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
DOCASSEMBLE --version
DOCASSEMBLE check-update
```

### Applying Updates
```bash
pip install --upgrade DOCASSEMBLE
```

### Rolling Back
```bash
pip install DOCASSEMBLE==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
