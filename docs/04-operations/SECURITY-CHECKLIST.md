# Security Checklist

## Goal
Provide a practical security baseline checklist for the Crystal Soul project.

## Local Development
- [ ] Use a separate local database for this project
- [ ] Keep local-only credentials out of Git
- [ ] Do not use production secrets in local environment
- [ ] Keep debug logging controlled
- [ ] Avoid installing unknown plugins/themes for testing without documentation

## WordPress Access
- [ ] Use a non-default admin username
- [ ] Use strong unique passwords
- [ ] Limit administrator accounts
- [ ] Review user roles before go-live
- [ ] Enable 2FA for production admin accounts

## Theme / Plugin Safety
- [ ] Never edit parent theme files
- [ ] Keep customizations in child theme or mu-plugin layer
- [ ] Remove unused plugins and themes
- [ ] Avoid overlapping plugins
- [ ] Update plugins/themes only after testing where possible

## Core Configuration
- [ ] Use HTTPS in production
- [ ] Set correct file permissions in production
- [ ] Disable debug display on production
- [ ] Protect sensitive configuration files
- [ ] Use secure backup storage outside the live server

## Backup / Recovery
- [ ] Define backup schedule
- [ ] Test restore process
- [ ] Keep at least one off-site backup
- [ ] Document backup ownership and access

## Monitoring / Operations
- [ ] Define update process
- [ ] Review logs when issues appear
- [ ] Use staging before risky changes
- [ ] Document incidents and fixes

## Git / Documentation Safety
- [ ] Do not commit secrets
- [ ] Keep `.gitignore` updated
- [ ] Document important security decisions
- [ ] Track plugin/security changes in docs
