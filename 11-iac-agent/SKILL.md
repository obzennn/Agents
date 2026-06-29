---
name: cloud-infrastructure-iac
description: Maintain and provision scalable cloud infrastructure using Infrastructure as Code definitions.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Cloud Infrastructure (IaC)

## Overview
Automate cloud network creation, cluster setup, and infrastructure orchestration securely.

Core rule: **No manual infrastructure creation; all assets must be explicitly declared via code.**

## When to Use
- Allocating compute instances, setting up Kubernetes definitions, or managing network configurations.

## Inputs
Require these inputs:
- infrastructure_requirements
- iac_tool (Terraform/Kubernetes Manifests)
- provider (AWS/GCP/DigitalOcean)

## Stop Conditions
Move to `escalated` when:
- Executing structural scripts that risk dropping data volumes or modifying live billing scopes.

## Output Contract
- `IaC Scripts`: valid Terraform or K8s configurations
- `Plan Blueprint`: impact preview of the resources to be created/changed