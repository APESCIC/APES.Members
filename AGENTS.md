# Agent instructions for APES.Members

Cursor's user rules and skills set how work is done here (branches, issues, pull requests, merge, release, deploy, ship gate, decisions and safety). This file describes this repository and fills the named slots below. If anything here disagrees with them, Cursor's rules win and this file is corrected in the same milestone.

Cursor/agent layout standard: https://github.com/apescic-director/Cursor/blob/main/docs/cursor-agent-standards.md

The owner is Bambie Murphy. Write UK English (organisation, behaviour, colour, licence) in the product, docs, issues and pull requests. Never print, paste or commit secrets.

## About the app

APES.Members is the planned APES CIC members area for member accounts, licence administration, adopt and foster applications, home checks, documents, notifications and payments. The repository is a scaffold today: only this guidance, ignore rules and a placeholder README are present. There is no application code, live URL or Cloudron app yet.

- Repository: `APESCIC/APES.Members`. Work only in this repository.

## Stack and architecture

Not chosen yet. When the app is scaffolded, record the languages, framework and key folders here. Area labels already reserved for the product include `area: accounts`, `area: licences`, `area: applications`, `area: home-checks`, `area: documents`, `area: notifications`, `area: payments`, `area: privacy`, `area: accessibility`, `area: infrastructure` and `area: docs`.

## Local development and preview

| Item | Value |
| --- | --- |
| Clone | `C:\Users\BambieMurphy\Documents\GitHub\APES.Members` |
| Herd site | None yet |
| Preview URL | None (scaffold only; skip the live preview gate until a Herd-served app exists) |
| Preview command | None |
| HMR port | None |
| Env file | None yet (when added, commit `.env.example` with key names only) |
| Database | None yet |
| Mail | None yet |

Laravel Herd is the only local stack once an app is present. Use fake demo data only; never real member, licence, application or payment data.

### Local development with Laravel Herd

When this repository gains a Herd-served site, run `herd site:info` for the URL, PHP version and connected services.

- Use `herd php` and `herd composer` so commands use this site's PHP version.
- Use `herd status` if something doesn't respond; `herd list` shows every command (`--json` for structured output).

## Tests and checks

| Check | Command |
| --- | --- |
| Tests | None yet |
| Lint / format | None yet |
| CI workflows | None yet (`.github/workflows/` when added) |

## Workflow slots

Shipping follows Cursor's `github-milestone-completion` and `ship-gate` skills. This repo fills these slots:

| Slot | Value |
| --- | --- |
| Milestone branch pattern | `milestone/vX-Y-Z-<slug>` (confirm when the first versioned milestone opens) |
| Version files | None yet |
| Release tooling | None yet |
| Area labels | `area: accounts`, `area: licences`, `area: applications`, `area: home-checks`, `area: documents`, `area: notifications`, `area: payments`, `area: privacy`, `area: accessibility`, `area: infrastructure`, `area: docs` |
| Issue title prefix | `[Type] Short title` |

Development is tracked only in GitHub issues, sub-issues and `vMAJOR.MINOR.PATCH` milestones — never Linear.

## Deploy and health

| Item | Value |
| --- | --- |
| Target | Not deployed |
| Cloudron app ID | None |
| Domain | None |
| Deploy command | None |
| Deploys | Not applicable until a Cloudron app and release process exist |
| Auto-deploy couplings | none |
| Health URL | None |
| Version field | None |
| Secrets live in | APES Vault (Bitwarden); never commit secrets |

## Decisions and gotchas

- 2026-11-16: Repository is a thin scaffold (README only). Agent layout brought into line with the APES Cursor/agent standard (`AGENTS.md` + `.cursorignore`). Decided as part of the org-wide Cursor config alignment.

## Where to find things

- Placeholder overview: [README.md](README.md)
- Org Cursor/agent standard: [docs/cursor-agent-standards.md](https://github.com/apescic-director/Cursor/blob/main/docs/cursor-agent-standards.md) in the Cursor ops hub
