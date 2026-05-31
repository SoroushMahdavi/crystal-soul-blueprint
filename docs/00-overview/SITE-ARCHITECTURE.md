# Site Architecture

## Goal
Define the high-level architecture of Crystal Soul (components + responsibilities) so the build stays consistent and maintainable.

---

## Environments
- **Local (XAMPP):** development + learning + testing
- **Staging (future):** pre-production testing
- **Production (future):** live store

Rule: features/settings must be validated on Local (and later Staging) before Production.

---

## Core Stack
- **CMS:** WordPress
- **E-commerce:** WooCommerce
- **Theme:** Woodmart (Parent) + Crystal Soul (Child)
- **Customization Layer:**
  - Child Theme for UI-level changes
  - MU Plugin for "must-run" logic (bootstrap tasks)
- **SEO:** Rank Math (planned)
- **Security:** Wordfence (planned for production)
- **Backups:** UpdraftPlus (planned for production)

---

## Responsibility Map

### WordPress Core
- users, roles, base settings
- content pages (About, Contact, Policies)
- media library

### WooCommerce
- products, pricing, stock
- checkout and customer account
- coupons
- shipping/tax configuration

### Theme (Woodmart)
- shop UI templates
- header/footer layouts
- product page layout baseline

### Child Theme (Crystal Soul)
- safe CSS/JS adjustments
- small UI behavior changes
- minimal WooCommerce template overrides (only when needed)

### MU Plugin (Bootstrap)
- one-time setup tasks
- default options/flags
- guardrails (idempotent logic)

---

## Data Model (Launch)
- Launch category: **Bracelets**
- Keep product model simple
- Use global attributes only when needed for filtering consistency

---

## Non-goals (Launch)
- Multi-language setup
- Advanced recommendation engine
- Complex membership/subscription systems
- Heavy page-builder dependency across the store

---

## Quality Rules
- Avoid plugin overlap
- Document changes before/after applying
- Keep rollback possible
- Prefer hooks over template overrides
