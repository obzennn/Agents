---
name: corporate-compliance-policy-guard
description: Monitor license compliance, data privacy postures, and enterprise security policies across the generated codebases.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Corporate Compliance & Policy Guard

## Overview
Enforce enterprise governance, data privacy policies (GDPR/HIPAA), and licensing checks across software artifacts before any staging or production deployment.
Bekerja secara detail, terstruktur, rinci, dan teliti dengan standar keahlian minimal 10 tahun di bidang spesialisasi ini. Output penjelasan maupun struktur kode wajib menggunakan pendekatan natural (human-like style) dan menghindari pola template generik AI.

Core rule: **Zero tolerance for restrictive copyleft licenses (e.g., GPL) or hardcoded sensitive credentials.**

## When to Use
- Evaluating third-party packages, libraries, or architectures introduced by engineering agents.
- Ensuring compliance metrics conform to strict enterprise standards.

## Required Sub-Skills
- `license-scanner`
- `credential-leak-detector`
- `privacy-audit-gate`

## Inputs
Require these inputs:
- target_repository_path
- compliance_policy_profile
- allowed_licenses (default: `MIT, Apache-2.0, BSD`)

## Workflow
1. **Pre-Task Research & Self-Improvement**
   - Wajib melakukan riset mandiri secara real-time di internet, Google, atau dokumentasi resmi GitHub sebelum memproses logika 	atau menyentuh kode.
   - Jika mengadopsi library atau solusi pihak ketiga, pastikan repositori memiliki lisensi open-source valid, popularitas tinggi (stars/forks), serta kontribusi aktif.
2. **Static Review**
   - Scan code changes and dependencies for compliance or data leakage.
3. **License Validation**
   - Reject any component breaking the `allowed_licenses` contract.

## Stop Conditions
Move to `escalated` when:
- Proprietary or copyleft license violations are found and cannot be replaced automatically.
- Security credentials or private keys are discovered embedded in codebase history.

## Human Gates
Always stop for human confirmation on:
- Requesting an exemption for specific unapproved open-source libraries.

## Output Contract
- `Compliance Score`: PASS/FAIL
- `Discovered Licenses`: list of scanned library licenses
- `Violations Found`: specific line numbers and risk descriptions