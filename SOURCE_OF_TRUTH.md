# SOURCE_OF_TRUTH.md — Little Fight NYC Website Template

Last verified: 2026-06-30 by Codex.

## Repository

- GitHub: `https://github.com/omgitsthedm/website-template.git`
- Default branch: `master`
- Canonical working path for this consolidation pass: `Brand/Internal/Shared/Shared/website-template`
- Consolidation branch: `codex/agency-standard-website-template-20260629`
- Backup branch for the original divergent local commit: `backup/consolidation-website-template-20260629`

## Production Linkage

- No production host or live URL is verified for this project.
- No build command is configured.
- No deploy mechanism is configured.
- Treat this as a reusable source template until David explicitly assigns a host or client target.

## Source Layout

- `index.html` — template homepage.
- `404.html` — static not-found page.
- `css/styles.css` — template styles.
- `js/main.js` — template behavior.
- `robots.txt` and `sitemap.xml` — starter public metadata.

## Clone Topology Observed

- `Brand/Internal/Shared/Shared/website-template`: had local commit `d91e4ce` diverged from `origin/master`; now used to build the consolidation branch.
- `Archive/website-template`: clean and aligned with current `origin/master` after fetch.
- `Brand/Internal/website-template`: clean but one commit behind `origin/master` after fetch.

## Safety Notes

- Do not force-push or rewrite `master`.
- Do not deploy or wire hosting without David approval.
- Keep this repo free of `.env`, secrets, dependency installs, and client-specific private data.

## Verification

- `agency-doctor --fix` installed the standard files and local pre-commit secret hook on the consolidation branch.
- Pending after commit: run `git diff --check`, run `agency-doctor`, and push the consolidation branch.
