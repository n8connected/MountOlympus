# Mount Olympus | Complete platform requirements

Status: specification only. Implemented functionality must be verified separately; do not label unbuilt integrations complete.

## Brand and layout
- Site: black #000000, white #FFFFFF, gold accent; X-like navigation and feed styling.
- Primary logo: Mount Olympus mountain wordmark.
- Site favicon and every app icon: Mount Olympus gold pillar.
- Small N8 mark appears ONLY near bottom-right install-updates area of Windows executables.
- Embed real Windows titlebar/taskbar icon, compact updates control and truthful update status.
- Windows native portable 64-bit GUI .exe is primary Windows deliverable, not scripts or source.

## Homepage / URL search
- Public searchable URL directory with title, category, tags, descriptions and safety checks.
- Voting (up/down), comments, sharing, content reporting and moderation.
- Premium accounts exclusively submit URLs via /upload.
- Direct video player for supported authorized sources; do not rip third-party streams.
- Guest/free downloads offered through policy-compliant opted-in rewarded advertising, including between downloads.
- Streaming ad formats subject to provider policy and actual inventory, not unilaterally enforced billing rules.
- AdSense and separately purchased on-site ad placements; advertisers have business registration, signed agreement, campaign dashboard, budgets, analytics, payment records.

## Accounts and profiles
- Email/password with verified email and secure password reset.
- Optional Google, Facebook and X sign-in; optional anonymous PGP login.
- Once PGP is established and verified, account uses PGP security flow and may display 'maximum security' profile badge.
- Encourage TOTP authenticator 2FA for others; recovery codes and secure session controls.
- Custom unique @handle, public profile route, uploaded avatar, social badges with platform logos and usernames.
- Featured affiliate URLs on profile.
- Refer4Refer category tables with switching tabs including YouTube Subscribe4Subscribe; anti-spam and third-party terms enforcement.
- Owner administrative access through verified challenge-response using user's PGP PUBLIC key. Never store private keys.

## User levels and pricing
- Guest: read/search, ad-gated download.
- Free: login/profile, comments/votes, ad-gated download; cannot upload URLs.
- Premium: initial month AUD $1.00; subsequent AUD $18.99/month billed AUD $56.97 every 3 months; premium URL uploads, no homepage ads, unlimited platform download count subject to fair-use and availability.
- Clear auto-renewal and cancellation controls; signed electronic waiver before Premium activation.
- No change-of-mind refunds, subject to non-excludable consumer rights under applicable law.
- Business advertisers must complete sign-up and electronically sign advertiser agreement.
- Audit waiver identity, timestamp, consent text, document hash, and version.

## Payments and revenue
- Integrate Square, Stripe, PayPal with securely processed webhooks, ledgers, reconciliation, disputes and subscription renewals; never ship secrets in clients.
- Separate income sources: premium subscription, direct ad sales and approved ad-network revenue.
- Verification and moderation for advertisers and URLs.

## Public navigation
- Search, Upload URL (premium), Stream, Download, Refer4Refer, Profiles, Advertise, Premium, How To, Sign in/up, About, Terms, Privacy.
- How To: sharing video via a supported URL; uploading/sharing URLs; accounts; social badges; ads; membership; download instructions.

## Admin dashboard
Blogger-style CMS with Posts, Pages, URLs, Moderation, Users, Roles, Accounts, Waivers/Signatures, Premium Billing, Advertisers, Campaigns, Ads, Streams, Downloads, API, Themes, Security, Audit Log, Settings.
Require separate permissions and safe authentication, never rely on client-side admin hiding.

## API / hosting
- Single shared database and backend API for all platforms.
- Local Windows master dashboard to configure domain and manage Cloudflare Tunnel with explicit Cloudflare authorization; TLS and origin security.
- User API integration settings, credential lifecycle and usage logs.
- Windows, macOS and Linux desktop clients; Microsoft Store, Chrome/Edge-compatible extension, Android Play Store and iOS App Store builds. Each requires its own signing/store validation.
- Site may be published through ChatGPT Sites if deployment tools and credentials are available. Avoid claiming deployment without verification.

## Release/update contract
- Signed/verified release manifests over HTTPS with semantic versions and integrity verification.
- In-app bottom-right N8 mark, Install Updates control and real update-availability notification.
- Never launch unverified downloads or treat an update URL opener as self-installation.
- Test Windows executable icon, PE subsystem, GUI launch, navigation, update check, backend, billing and auth end to end; report missing tests.

## Outstanding deliverables
Production backend integration, OAuth/PGP/TOTP recovery, payment providers, compliant video/advertising, waivers, protected upload moderation, Cloudflare automated provisioning, app signing, store builds, GitHub release and Windows runtime testing.
