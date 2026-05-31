# Git and Deployment Workflow

## Goal
Keep a clean, low-risk workflow for documentation + future code changes.

---

## Repository Scope
This repo is for:
- documentation (Markdown)
- small code artifacts (child theme snippets, mu-plugin code) if needed later

This repo is NOT for:
- full WordPress core files
- wp-content uploads
- database dumps with real data

---

## Branching Policy (Simple)
- `main` is stable
- work directly on `main` for docs (for now)
- if code changes increase, introduce feature branches:
  - `feature/<name>`

---

## Commit Rules
- small commits
- clear messages
- one theme per commit

Examples:
- `Add batch 3 architecture and roadmap docs`
- `Update product attribute policy`
- `Document WooCommerce setup decisions`

---

## Deployment Philosophy (Future)
- Local → Staging → Production
- Never change production first
- Document steps before execution
- Maintain rollback plan

---

## What we track in docs
- plugin changes
- theme changes
- WooCommerce settings decisions
- data model changes (categories/attributes)
- incidents and fixes

---

## Security Notes
- never commit secrets
- keep `.gitignore` strict
- access to repo should be limited
