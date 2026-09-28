# Project State

## Objective

Publish a minimal public homepage and privacy policy for the private Jarvis Google OAuth client, without exposing personal or project information.

## Current state

- Public repository created at `cluelessbk/jarvis-site`; GitHub Pages build is successful.
- `jarvis.wardiel.com` points to GitHub Pages through a DNS-only Cloudflare CNAME.
- Homepage and privacy policy are publicly available over HTTP; GitHub certificate issuance is pending before HTTPS enforcement can be enabled.
- Search indexing is discouraged through page-level `noindex` directives and `robots.txt`.
- No analytics, tracking, personal details, or project information is included.
- Google OAuth Branding uses the homepage/privacy URLs and lists `wardiel.com` as an authorized domain.
- OAuth publishing status is `In production`.
- A fresh production-mode Gmail token was issued with Gmail send, Gmail modify, and Pub/Sub scopes; the Gmail profile check and watch renewal succeeded.

## Next action

Wait for GitHub's certificate issuance, enable HTTPS enforcement, and verify both public pages over HTTPS.

## Blockers

- GitHub is still provisioning the custom-domain TLS certificate.
- Google reports that the sensitive/restricted scopes require verification. This does not prevent the single authorized account from using the app in Production, but it retains the unverified-app warning and 100-user lifetime cap.
