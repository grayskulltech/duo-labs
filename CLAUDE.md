# Duo Labs

## IP Classification
- **Owner:** Grayskull Technology LLC (commercial IP)
- **Data Classification:** INTERNAL (lab configs), CONFIDENTIAL (any customer-specific PoC data)
- **Never** commit customer names, AKEYs, or real environment data. Use sanitized examples.

## Project Overview
Lab configurations and PoC/PoV demos for Duo Security. Contains reference architectures, demo scripts, and proof-of-concept integrations for customer engagements.

## Structure
- Lab configs: Docker Compose, Terraform, or manual setup docs
- Each lab/demo in its own directory with a README
- Demo data must be synthetic — no real customer data

## Code Quality
- All demo scripts must work on Windows (Git Bash or PowerShell).
- Docker Compose files: validate with `docker compose config` before committing.
- Environment variables for all credentials — never hardcoded.
- README per lab: purpose, prerequisites, setup steps, teardown steps.

## Sensitive Files (do not commit)
- `.env` — credentials for lab environments
- Any file containing real customer data
- Duo integration keys (IKEYs, SKEYs, AKEYs)
