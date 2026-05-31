# HOSTING-DOMAIN-SECURITY – Crystal Soul

## Purpose
This file defines the baseline guidance for hosting, domain, and core security decisions for the Crystal Soul project.

---

## 1) Hosting Comparison

### Option A: Liara
#### Pros
- Good local/Iranian infrastructure access
- Easier local payment and support flow
- Suitable for lightweight regional projects
- Simpler onboarding for Persian-speaking operators

#### Cons
- Not the best fit for a WooCommerce store targeting Canada
- International performance and global routing may be less optimal
- WordPress/WooCommerce ecosystem flexibility may be lower than specialized global providers
- Some advanced hosting workflows may be more limited than international managed providers

#### Best Use Case
- Iran-first projects
- Lower-complexity deployments
- Teams prioritizing local support over international optimization

---

### Option B: ParsPack
#### Pros
- Familiar local hosting provider
- Easier billing and support for Iran-based operators
- Useful for smaller projects or local-market launches
- Often easier for domain/DNS management within Iran

#### Cons
- Less ideal for a store whose main customer base is in Canada
- Managed WooCommerce optimization may not be as strong as specialized providers
- Global CDN/performance strategy may require extra layers
- Long-term scaling for international ecommerce may be less elegant

#### Best Use Case
- Budget-sensitive local projects
- Teams wanting local provider convenience
- Initial low-scale deployment

---

### Option C: ArvanCloud
#### Pros
- Strong infrastructure and CDN-related ecosystem
- Better performance architecture than many basic local hosts
- Can be useful when network/security layer matters
- Potentially good if combined intelligently with other infrastructure choices

#### Cons
- May require more technical handling depending on architecture
- Not a “simple managed WooCommerce” experience by default
- For non-developers, setup may feel less straightforward than managed WordPress platforms
- International ecommerce convenience still may not match top global managed WP providers

#### Best Use Case
- Teams comfortable with infrastructure decisions
- Projects needing stronger network-layer thinking
- Hybrid/local-cloud architectures

---

### Option D: Cloudways
#### Pros
- Strong balance of flexibility and managed hosting convenience
- Very suitable for WooCommerce
- Easy scaling compared to many budget/shared hosts
- Better environment separation possibilities (staging, production)
- More developer-friendly than many beginner-only hosts
- Good fit for international/Canada-focused ecommerce
- Stronger control without needing to manage raw infrastructure directly

#### Cons
- More expensive than many local options
- Requires some familiarity with hosting concepts
- Add-ons and premium features may increase recurring cost
- Still not as “fully hands-off” as some highly opinionated managed platforms

#### Best Use Case
- Serious WooCommerce projects
- International stores
- Teams wanting flexibility + managed convenience
- Best balance for technical users who are not full-time WP developers

---

### Option E: SiteGround
#### Pros
- Well-known managed WordPress provider
- User-friendly panel and workflows
- Good support reputation
- Easier for standard WordPress operations
- Suitable for small to medium stores with lower technical overhead

#### Cons
- Can become expensive for what it offers at higher tiers
- May feel more restrictive than Cloudways for technical users
- Resource limits and scaling model may become less attractive over time
- For WooCommerce growth, cost/performance ratio should be evaluated carefully

#### Best Use Case
- Users wanting simpler managed hosting
- Smaller to medium WooCommerce stores
- Teams preferring ease of use over flexibility

---

## 2) Hosting Recommendation

### Recommended Default: Cloudways
#### Why
For Crystal Soul, Cloudways is the strongest default recommendation because:
- the target market is Canada, not Iran
- WooCommerce needs stable performance and scaling headroom
- the project requires maintainability and safer environment separation
- you have enough technical understanding to benefit from Cloudways without being blocked by its complexity
- it provides a better long-term base for growth than typical local hosting

### Recommended Alternative
#### SiteGround
Choose SiteGround if:
- you want a simpler managed experience
- you prefer easier hosting workflows over flexibility
- the store remains relatively small in the first phase

### Conditional Local Option
Use Liara / ParsPack / ArvanCloud only if:
- budget pressure is high
- launch must be heavily localized operationally
- or there is a strong reason to keep hosting stack inside the Iranian ecosystem

For a Canada-focused ecommerce brand, local hosting is generally not the default recommendation.

---

## 3) Domain Strategy

### .com vs .ir

#### .com
##### Pros
- Best for international credibility
- Stronger fit for Canada/global audience
- Better brand portability
- Cleaner for future expansion
- Preferred default for ecommerce targeting international customers

##### Cons
- Desired names may be less available
- Usually slightly more expensive than .ir
- Requires stronger brand-name selection due to availability competition

#### .ir
##### Pros
- Useful for Iran-facing identity
- Often easier and cheaper to register
- Can be useful as a defensive or secondary domain

##### Cons
- Weaker fit for Canada-first branding
- Less ideal for international trust and perception
- Not the best primary identity for a globally oriented store

---

## 4) Domain Recommendation

### Primary Recommendation
Use a `.com` domain as the primary domain.

### Secondary Recommendation
If relevant and available, also register the `.ir` version defensively and redirect or reserve it.

### Naming Direction
Brand naming should align with:
- calm
- spiritual/lifestyle feel
- premium handmade positioning
- memorability in English-speaking markets

Potential naming direction:
- crystalsoul.com
- crystalsoulshop.com
- crystalsoulstudio.com
- mycrystalsoul.com
- crystalsoulcollective.com

If the exact preferred name is unavailable, keep the name:
- short
- brandable
- easy to spell
- internationally readable

---

## 5) Core Security Baseline

### SSL
#### Free SSL
Example: Let’s Encrypt

##### Pros
- Usually sufficient for most ecommerce stores
- Encrypts traffic properly
- Good default for launch
- Cost-effective

##### Cons
- Some setups require more manual renewal awareness
- Does not itself add trust signals beyond encryption

#### Paid SSL
##### Pros
- Can provide brand/organization validation depending on type
- Sometimes useful for enterprise or specific compliance expectations

##### Cons
- Often unnecessary for a standard WooCommerce launch
- Adds cost with limited practical benefit for many small/medium stores

### SSL Recommendation
Use free SSL by default unless a specific business/compliance need justifies paid SSL.

---

### WAF / CDN
#### Recommended Layer: Cloudflare
##### Why it matters
- Improves security posture
- Adds DDoS and traffic filtering benefits
- Helps caching and global performance
- Useful especially for internationally accessed stores

### WAF Recommendation
Use Cloudflare as the default external protection/performance layer.

---

### Backups
Backups are mandatory.

#### Requirements
- automatic scheduled backups
- off-site storage
- ability to restore specific files/database
- restore testing, not just backup creation

#### Why it matters
Backups protect against:
- failed plugin/theme updates
- malware/compromise
- operator mistakes
- hosting failures
- data corruption

---

## 6) Security Priority Checklist

### Recommended
- SSL enabled
- Cloudflare configured
- automatic backups enabled
- off-site backup storage configured
- strong admin password policy
- two-factor authentication for admins
- least-privilege admin access
- regular update policy
- staging before major changes

### Optional
- paid SSL if business case exists
- advanced malware scanning layer
- server-side hardening beyond hosting defaults

### Risky / Avoid
- relying only on host-level backups
- storing backups only on the same server
- making major plugin/theme updates directly on production first
- using weak/shared admin credentials

---

## 7) Current Default Decision
Unless future project constraints override it:

- Primary hosting recommendation: Cloudways
- Simpler alternative: SiteGround
- Primary domain: `.com`
- Defensive secondary domain: `.ir` if useful
- SSL: free SSL by default
- WAF/CDN: Cloudflare
- Backups: automatic + off-site + restore-tested
