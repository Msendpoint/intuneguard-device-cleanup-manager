# IntuneGuard

> A multi-tenant Intune device hygiene SaaS that audits, enforces, and reports on stale device cleanup policies so MSPs never lose compliance visibility again.

## Overview

IntuneGuard connects to multiple Microsoft 365 tenants via Graph API and continuously monitors Intune cleanup rule configurations, flagging drift from a defined policy baseline and generating scheduled stale-device reports. MSPs and enterprise IT teams get a single dashboard showing which tenants have misconfigured cleanup windows, how many ghost devices are polluting each environment, and a one-click remediation to enforce consistent settings across all tenants at once.

## Problem This Solves

There is no native audit trail or multi-tenant enforcement mechanism for Intune device cleanup rules, so MSPs manually re-check portal settings across dozens of clients and routinely discover stale ghost devices inflating license counts and breaking dynamic group targeting only after compliance reports are already wrong

## Target Audience

MSP technicians and enterprise Intune admins managing 3+ tenants with 200+ devices each, who are responsible for compliance reporting and license cost control

## Tech Stack

PowerShell, Next.js, Node.js, Microsoft Graph API, PostgreSQL, Stripe, Vercel

## Installation

```powershell
# Clone the repository
git clone https://github.com/intuneguard-device-cleanup-manager.git
cd intuneguard-device-cleanup-manager

# Review the script before running
Get-Content scripts/intuneguard-device-cleanup-manager.ps1

# Run with appropriate permissions
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\scripts\{intuneguard-device-cleanup-manager}.ps1
```

## Usage



## Monetization Strategy

SaaS subscription sold via Stripe on a self-hosted or Vercel-deployed web app: Starter (up to 3 tenants) at $29/month, Pro (up to 15 tenants) at $79/month, Agency (unlimited tenants + white-label PDF reports) at $199/month. Launch with a Gumroad-sold standalone PowerShell toolkit at $49 one-time to validate demand and build an email list before launching the SaaS.

| Metric | Value |
|--------|-------|
| Revenue Potential | HIGH |
| Estimated Effort  | 1-3months |

## Contributing

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*Generated from the article: [Automate Intune Device Cleanup Rules with PowerShell](https://msendpoint.com/articles/automate-intune-device-cleanup-rules-with-powershell) on 2026-03-28*
*Blog: [MSEndpoint.com](https://msendpoint.com)*