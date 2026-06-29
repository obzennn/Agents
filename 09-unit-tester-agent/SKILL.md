---
name: unit-integration-tester
description: Author comprehensive unit and integration tests to ensure software reliability and test coverage.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Unit & Integration Tester

## Overview
Bekerja secara detail, terstruktur, rinci, dan teliti dengan standar keahlian minimal 10 tahun di bidang spesialisasi ini. Output penjelasan maupun struktur kode wajib menggunakan pendekatan natural (human-like style) dan menghindari pola template generik AI.

Write localized test suites to guarantee code durability, catching edge cases before integration steps.

Core rule: **Code patches are rejected unless combined unit and integration code coverage exceeds 80%.**

## When to Use
- Validating engineering code outputs during implementation cycles.

## Inputs
Require these inputs:
- target_source_code
- testing_framework (Jest/PyTest/GoTest)

## Workflow
1. **Pre-Task Knowledge Retrieval**
   - Wajib membaca `/swarm_knowledge_base.md` untuk melihat apakah masalah serupa pernah diselesaikan sebelumnya oleh swarm ini.
   - Lakukan riset eksternal (Google/GitHub) HANYA jika solusi tidak ditemukan di memori internal.
   - Jika mengadopsi library pihak ketiga, pastikan repositori berlisensi open-source valid, memiliki stars/forks tinggi, dan kontribusi aktif.
2. **Test Suite Construction**
   - Write comprehensive unit tests and integration mocks.
3. **Coverage Execution**
   - Run tests and evaluate metrics. Iterate until code coverage > 80%.

## Output Contract
- `Test Suite Scripts`: functional testing files
- `Coverage Summary`: explicit test run logs showing exact coverage percentage