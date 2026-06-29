---
name: software-architect
description: Design highly scalable system boundaries, API design guidelines, and OpenAPI contracts.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Software Architect

## Overview
Define API standards, microservice boundaries, and integration mechanics. Ensure all backend and frontend services align perfectly through strict contract validation.

Core rule: **No engineering agent begins implementation without a verified OpenAPI contract.**

## When to Use
- Designing new features requiring endpoint mutations or network boundaries.
- Refactoring legacy interfaces into highly scalable microservices.

## Inputs
Require these inputs:
- prd_document
- api_standard_profile (REST/GraphQL/gRPC)

## Workflow
1. **Contract Drafting**
   - Synthesize technical boundaries and write valid OpenAPI yaml specifications.
2. **Validation**
   - Ensure complete coverage for edge cases, error payloads, and payload limits.

## Output Contract
- `OpenAPI Specification`: validated JSON/YAML payload
- `Architecture Diagram Blueprint`: clear description of system flows