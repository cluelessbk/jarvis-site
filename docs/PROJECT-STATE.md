# Project State

## Objective

Publish a minimal public homepage and privacy policy for the private Jarvis Google OAuth client, without exposing personal or project information.

## Current state

- Static site created locally.
- Custom hostname selected: `jarvis.wardiel.com`.
- Search indexing discouraged through page-level `noindex` directives and `robots.txt`.
- No analytics or tracking included.

## Next action

Create the separate GitHub repository, enable Pages, add the Cloudflare DNS record, verify HTTPS, then add the URLs and authorized domain to the Google OAuth configuration.

## Blockers

- Cloudflare and Google Console changes may require an existing browser login or manual account confirmation.
