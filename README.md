# Mount Olympus

Mount Olympus is a URL-sharing, search, streaming and member community platform.

## Windows Master Dashboard
Native Windows 64-bit GUI application. The window and taskbar use the Mount Olympus pillar icon. A small N8 logo sits beside the update checker in the lower-right corner.

The current local GUI executable is **not** the complete platform backend. It can open configured site routes and inspect a site's update manifest, but hosted services, identity providers, payment processors and streaming require implementation and deployment.

### Branding
- Background: `#000000`
- Text: `#FFFFFF`
- Accent: gold
- App icon: Mount Olympus pillar
- Tiny update-area mark: N8

### URL sharing and community
- Search, vote up/down, comments, share URL, moderation
- Premium-only URL submissions, profiles and custom @handles
- Social platform badges and featured affiliate links
- Refer4Refer category tabs for social platform sharing
- Guest and free accounts with appropriately approved rewarded advertising; paid tier with no homepage ads

### Accounts
- Email/password, email reset, authenticator 2FA; optional PGP authentication and stronger profile badge
- Google, Facebook and X identity providers (requires provider integration)
- Owner administrator authenticated by assigned PGP public key and verified private-key challenge
- Waiver signing required for paid memberships and advertisers

### Commercial rules
- Month one: AUD $1
- From month two: AUD $18.99 per month, billed every three months (AUD $56.97 per quarter)
- No change-of-mind refunds; statutory consumer rights remain
- Square, Stripe, PayPal integration planned; Google advertising and direct advertiser marketplace planned

### Applications
- Native Windows dashboard; proposed desktop apps for Linux/macOS, browser extension, Android and iOS clients
- One central backend/API and account database; Cloudflare Tunnel management planned

## Update endpoint
A future hosted backend may expose `/updates/windows.ini`:

```ini
[Update]
Version=2.0.0
DownloadURL=https://example.com/releases/MountOlympus-Master.exe
```

**Security:** A manifest only announces an update. Production installer must require HTTPS, authentic release signing/checksums, semantic version comparison and explicit user consent before running downloads. Do not treat this draft protocol as a safe unattended installer.

## Implementation status
This repository is the project documentation entry point. The current executable is compiled in the workspace but has not been Windows runtime-tested or published as a GitHub release. Deployment and the production backend remain incomplete.
