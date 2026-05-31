# WordPress + WooCommerce Install Checklist (XAMPP)

## Goal
Provide a repeatable installation checklist for local setup on XAMPP.

## Stage 1 — Local Folder Structure
- [ ] Create a dedicated project folder:
  - `C:\xampp\htdocs\crystal-soul`
- [ ] Place WordPress files inside that folder
- [ ] Confirm site path target:
  - `http://localhost/crystal-soul`

## Stage 2 — Database
- [ ] Open phpMyAdmin
- [ ] Create database:
  - `crystal_soul_local`
- [ ] Use `utf8mb4` collation if available
- [ ] Keep local DB isolated from other projects

## Stage 3 — WordPress Install
- [ ] Open `http://localhost/crystal-soul`
- [ ] Select language
- [ ] Enter database credentials
- [ ] Complete WordPress installation
- [ ] Use a non-default admin username
- [ ] Store credentials safely outside Git

## Stage 4 — Basic WordPress Settings
- [ ] Set site title
- [ ] Set timezone
- [ ] Review permalink structure
- [ ] Review discussion/comment settings
- [ ] Remove sample content if not needed

## Stage 5 — WooCommerce Install
- [ ] Install and activate WooCommerce
- [ ] Complete minimal setup wizard
- [ ] Set store country/region
- [ ] Set currency
- [ ] Review shipping needs
- [ ] Review tax approach
- [ ] Confirm account/cart/checkout pages exist

## Stage 6 — Theme Setup
- [ ] Install Woodmart parent theme
- [ ] Install required companion components
- [ ] Install Crystal Soul child theme
- [ ] Activate child theme
- [ ] Avoid direct parent theme edits

## Stage 7 — Plugin Baseline
- [ ] Install only approved plugins
- [ ] Do not install overlapping SEO/cache/security tools
- [ ] Document each plugin purpose

## Stage 8 — Product Foundation
- [ ] Create product category: Bracelets
- [ ] Create agreed global attributes
- [ ] Define SKU pattern
- [ ] Upload optimized sample product images
- [ ] Add 1–2 test products first

## Stage 9 — Local Validation
- [ ] Test homepage access
- [ ] Test shop page
- [ ] Test single product page
- [ ] Test add-to-cart flow
- [ ] Confirm no major PHP warnings in debug log
