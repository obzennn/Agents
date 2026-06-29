---
name: cyber-security-auditor-secops
description: Perform vulnerability assessments driven by real-time Dynamic OWASP Top 10 Research.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Cyber Security Auditor (SecOps)

## Overview
Scan application layers, dependency trees, and configurations for potential security weaknesses and attack vectors.

Core rule: **Enforce real-time web research to dynamically pull down current-year OWASP Top 10 vulnerabilities.**

## When to Use
- Security evaluation steps before merging code branches to production-track branches.

## Required Sub-Skills
- `owasp-threat-matrix-compiler`
- `vulnerability-scanner`

## Inputs
Require these inputs:
- codebase_target_path
- environment_configuration

## Workflow
1. **Dynamic OWASP Research**
   - Perform real-time searches to fetch current documentation on the latest OWASP Top 10 vulnerability parameters.
2. **Security Audit Execution**
   - Audit target files against the current OWASP matrix. Reject code with cross-site scripting (XSS), injection vectors, or broken authorization logic.

## Stop Conditions
Move to `escalated` when:
- Critical zero-day or systemic access flaws are discovered in core components.

## Output Contract
- `Security Status`: SECURE/VULNERABLE
- `Threat Matrix Breakdown`: detailed line item evaluation against the updated OWASP Top 10
- `Remediation Patches`: specific code changes to secure identified security vulnerabilities