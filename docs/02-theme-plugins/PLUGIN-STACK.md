# Plugin Stack Policy

## Goal
Define which plugins are approved, conditional, or avoided for the Crystal Soul project.

## Principles
- keep plugin count low
- avoid overlap
- prefer stable and well-supported plugins
- document why each plugin exists
- uninstall unused plugins

---

## Mandatory / Core Plugins

### WooCommerce
- **Role:** Core ecommerce platform
- **Status:** Mandatory

### Woodmart Core-related Components
- **Role:** Theme-required companion functionality
- **Status:** Mandatory if required by theme version
- **Note:** Only install components actually required by the active theme version

---

## Approved / Planned Plugins

### Rank Math
- **Role:** SEO
- **Status:** Approved
- **Reason:** Single SEO solution preferred

### Gravity Forms
- **Role:** Advanced forms for future guided tools / birth-month flow
- **Status:** Approved for future phase
- **Reason:** Strong conditional logic and extensibility

### WP Rocket
- **Role:** Caching / performance
- **Status:** Approved for production/staging planning
- **Reason:** Keep performance tooling centralized

### Wordfence
- **Role:** Security baseline
- **Status:** Approved for production planning
- **Reason:** Firewall / login protection / scanning baseline

### UpdraftPlus
- **Role:** Backup
- **Status:** Approved
- **Reason:** Clear backup/restore workflow

---

## Conditional Plugins

### Payment Gateway Plugin
- **Role:** Payment processing
- **Status:** Conditional
- **Rule:** Choose only one gateway stack per real business flow

### SMTP Plugin
- **Role:** Reliable email delivery
- **Status:** Conditional
- **Rule:** Add only when environment requires controlled email sending

### Image Optimization Plugin
- **Role:** Media optimization
- **Status:** Conditional
- **Rule:** Avoid overlap with caching/performance stack

---

## Avoid / Rejected Plugins

### Yoast SEO
- **Reason:** Overlaps with Rank Math

### Multiple Cache Plugins
- **Reason:** Conflict risk and unstable performance

### Multiple Security Plugins
- **Reason:** Conflict risk and unnecessary duplication

### Multiple Page Builders
- **Reason:** Design inconsistency, maintenance overhead, performance cost

### Random Snippet Plugins for Permanent Logic
- **Reason:** Permanent logic should live in child theme or mu-plugin layer when possible

---

## Operational Rules
- Every plugin must have a documented purpose
- Test new plugins locally before wider use
- Prefer no plugin over low-quality plugin
- Remove inactive/unneeded plugins
- Review plugin stack regularly
