# AGENTS.md — Little Fight NYC Website Template

> Shared repo instructions for Codex, Claude Code, and humans.

## What this is

- **Project:** reusable Little Fight NYC static website starter template.
- **Live URL:** none verified; this is a source template, not a deployed client site.
- **Stack:** static HTML/CSS/JS with no package manager, build step, or runtime backend.

## Source of truth

- GitHub remote: `https://github.com/omgitsthedm/website-template.git`.
- Default branch is `master`.
- This consolidation branch combines current `origin/master` with the local production-ready template commit that was previously only in `Brand/Internal/Shared/Shared/website-template`.
- Deeper provenance notes live in `SOURCE_OF_TRUTH.md`.

## Commands

- Preview: serve the repo root with any static server, for example `python3 -m http.server 4173`.
- Build: none.
- Lint/format: none configured.
- Deploy: none. Do not wire or deploy this template without David approval.

## Secrets

- Real secrets do not belong in this repo.
- `.env*`, dependency folders, and build outputs are ignored.
- The local pre-commit hook installed by `agency-doctor` blocks obvious secret commits.

## Before You Start

1. Check `git status --short --branch`.
2. Read this file and `SOURCE_OF_TRUTH.md`.
3. Use a branch for changes; do not rewrite `master`.
4. Keep template changes generic and reusable, not client-specific.

## Before You Finish

1. Run `git diff --check`.
2. If HTML/CSS/JS changed, preview the static site locally.
3. Update `SOURCE_OF_TRUTH.md` when source, branch, or clone-topology facts change.
4. Commit and push a branch; do not force-push.

## Do Not Touch Without Asking

- Deploy wiring, GitHub default-branch changes, destructive archive cleanup, or client-specific branding.

## Decisions Log

| Date | Decision | Why |
|------|----------|-----|
| 2026-06-30 | `codex/agency-standard-website-template-20260629` is the consolidation branch. | Preserves the local production-ready template commit on top of current `origin/master` without rewriting `master`. |
