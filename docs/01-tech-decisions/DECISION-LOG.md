# Decision Log

## Goal
Record important technical decisions for the Crystal Soul project in a structured, reviewable way.

## Usage Rules
- Add a new entry when a meaningful technical or operational decision is finalized.
- Keep entries short and clear.
- Include rejected alternatives where useful.
- Do not rewrite old entries unless the decision is officially changed.

---

## Entry 001 — Core Platform
- **Status:** Confirmed
- **Decision:** Use WordPress + WooCommerce as the project platform.
- **Why:** Strong ecosystem, fast MVP path, acceptable flexibility, easier maintenance than Magento for this phase.
- **Trade-offs:** Requires plugin discipline and regular maintenance.
- **Alternatives Considered:** Magento, Shopify

## Entry 002 — Primary Theme
- **Status:** Confirmed
- **Decision:** Use Woodmart as the main theme.
- **Why:** Strong WooCommerce support, suitable visual quality, flexible for premium product presentation.
- **Trade-offs:** Can become heavy if too many features/builders are enabled.
- **Alternatives Considered:** Flatsome, Luxolite

## Entry 003 — Theme Customization Strategy
- **Status:** Confirmed
- **Decision:** All safe customizations must go through the child theme.
- **Why:** Update safety and maintainability.
- **Trade-offs:** Requires a little more structure and discipline.
- **Alternatives Considered:** Direct parent theme edits, plugin-heavy customization

## Entry 004 — Environment Strategy
- **Status:** Confirmed
- **Decision:** Use XAMPP for local development.
- **Why:** Simple, familiar, and enough for early project phases.
- **Trade-offs:** Less portable than Docker-based environments.
- **Alternatives Considered:** Docker, LocalWP, Laragon

## Entry 005 — Launch Scope
- **Status:** Confirmed
- **Decision:** Initial launch focuses on bracelet products only.
- **Why:** Keeps catalog structure, UX, and data model simple for MVP.
- **Trade-offs:** Some future categories will need later expansion.
- **Alternatives Considered:** Multi-category launch from day one

## Entry 006 — Product Model Strategy
- **Status:** Confirmed
- **Decision:** Start with a simple product model and only introduce variations when genuinely needed.
- **Why:** Reduces admin complexity and avoids early catalog confusion.
- **Trade-offs:** Some future product flexibility may need restructuring.
- **Alternatives Considered:** Heavy variable-product-first approach

## Entry 007 — Bootstrap Strategy
- **Status:** Confirmed
- **Decision:** Maintain a documented one-time bootstrap plan for each fresh installation.
- **Why:** Reduces setup inconsistency and makes the system reproducible.
- **Trade-offs:** Requires up-front documentation effort.
- **Alternatives Considered:** Ad-hoc manual setup

## Entry 008 — Plugin Policy
- **Status:** Confirmed
- **Decision:** Keep plugin stack minimal and avoid overlapping functionality.
- **Why:** Better maintainability, lower conflict risk, cleaner performance baseline.
- **Trade-offs:** May require custom implementation in some areas.
- **Alternatives Considered:** Convenience-first plugin stacking
