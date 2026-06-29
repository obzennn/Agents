---
name: cloud-infrastructure-iac
description: Maintain and provision scalable cloud infrastructure using Infrastructure as Code definitions.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Cloud Infrastructure (IaC)

## Overview
Bekerja secara detail, terstruktur, rinci, dan teliti dengan standar keahlian minimal 10 tahun di bidang spesialisasi ini. Output penjelasan maupun struktur kode wajib menggunakan pendekatan natural (human-like style) dan menghindari pola template generik AI.

Automate cloud network creation, cluster setup, and infrastructure orchestration securely.

Core rule: **No manual infrastructure creation; all assets must be explicitly declared via code.**

## When to Use
- Allocating compute instances, setting up Kubernetes definitions, or managing network configurations.

## Inputs
Require these inputs:
- infrastructure_requirements
- iac_tool (Terraform/Kubernetes Manifests)
- provider (AWS/GCP/DigitalOcean)

## Workflow
1. **Pre-Task Research & Self-Improvement**
   - Wajib melakukan riset mandiri secara real-time di internet, Google, atau dokumentasi resmi GitHub sebelum memproses logika atau menyentuh kode.
   - Jika mengadopsi library atau solusi pihak ketiga, pastikan repositori memiliki lisensi open-source valid, popularitas tinggi (stars/forks), serta kontribusi aktif.

## Stop Conditions
Move to `escalated` when:
- Executing structural scripts that risk dropping data volumes or modifying live billing scopes.

## Output Contract
- `IaC Scripts`: valid Terraform or K8s configurations
- `Plan Blueprint`: impact preview of the resources to be created/changed