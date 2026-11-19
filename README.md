# Enterprise Cloud Security Lab

**Azure-First | AWS | Infrastructure Security | Terraform | DevSecOps**

## Overview

This repository documents the design and progressive implementation of an enterprise-style cloud security environment.

The lab simulates an organization with centralized security services, isolated development, testing, and production-like environments, secure identity management, infrastructure automation, and security monitoring.

**Current Status: Architecture Planning — Infrastructure Not Yet Deployed**

## Architecture

The initial design uses Azure hub-and-spoke networking.

- **Hub:** Centralized firewall, routing, DNS, and connectivity services.
- **Development Spoke:** Controlled infrastructure experimentation.
- **Testing Spoke:** Security and configuration validation.
- **Production-Like Spoke:** More restrictive security controls and change management.

The architecture will expand to include Azure identity security, governance, detection engineering, Kubernetes, and AWS infrastructure security.

[Read the Architecture Document](docs/architecture.md)

## Repository Structure

| Directory | Purpose |
|---|---|
| `docs/` | Architecture and security decisions |
| `terraform/` | Infrastructure as Code |
| `scripts/` | Automation and supporting tools |
| `validation/` | Functional and security testing evidence |
| `troubleshooting/` | Root-cause analysis and remediation |

## Engineering Approach

Every major implementation follows:

**Design → Build → Inspect → Test → Troubleshoot → Secure → Automate → Document**

Security controls will be validated before projects are marked complete.

## Project Status

The lab is currently in the architecture planning stage. No deployment is claimed.

Completed implementations, sanitized configuration examples, testing evidence, and lessons learned will be added progressively.

## Related Repositories

- [Professional GitHub Profile](https://github.com/cloud-sec-eng)
- [Cloud Security Portfolio](https://github.com/cloud-sec-eng/cloud-security-portfolio)

## Security Notice

This repository contains educational infrastructure configurations and sanitized engineering documentation.

Credentials, private keys, Terraform state, and sensitive infrastructure details must not be committed.
