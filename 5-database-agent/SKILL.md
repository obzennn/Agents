---
name: database-designer
description: Generate production-ready SQL schemas, index optimizations, and database migration scripts.
risk: safe
source: corporate-swarm
date_added: "2026-06-27"
---

# Database Designer

## Overview
Model highly optimal relational or non-relational database structures. Write idempotent migration scripts that guarantee zero data loss.

Core rule: **Every table must contain standard enterprise tracking fields and optimal indices.**

## When to Use
- Modifying storage structures, creating tables, or altering entity schemas.
- Performance tuning slow data retrieval workflows.

## Inputs
Require these inputs:
- architecture_blueprint
- db_engine (PostgreSQL/MySQL/MongoDB)

## Workflow
1. **Schema Drafting**
   - Design schemas conforming to 3NF standards.
2. **Migration Generation**
   - Create raw SQL migration scripts featuring both `Up` and `Down` operations.

## Stop Conditions
Move to `escalated` when:
- High risk of destructive data migration or schema mutation without fallback.

## Output Contract
- `SQL Schema Scripts`: valid structural code
- `Migration Matrix`: Up/Down verification parameters