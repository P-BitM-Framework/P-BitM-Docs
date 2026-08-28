# Contributing to the P-BitM documentation

Thank you for helping make P-BitM safer and easier to operate. Contributions
should be focused, verifiable against the current
[P-BitM source](https://github.com/P-BitM-Framework/P-BitM), and suitable for
authorized security assessments.

## Before starting

- Search existing issues and pull requests.
- Open an issue before a substantial reorganization or new documentation area.
- Keep unrelated rewrites out of focused fixes.
- Base behavioral claims, defaults, limits, and commands on the current P-BitM
  code, configuration, or tests.
- Read [STYLE_GUIDE.md](STYLE_GUIDE.md).

## Local preview

Install Node.js 20.17.0 or newer and the current documentation CLI:

```bash
npm install --global mint
mint dev
```

Before opening a pull request, run:

```bash
mint validate
mint broken-links --check-anchors
mint a11y
git diff --check
```

If a check cannot be run, explain why in the pull request.

## Content requirements

- Write public documentation in English.
- Add `title` and `description` frontmatter to every published MDX page.
- Add new pages to `docs.json` and use root-relative internal links.
- Keep examples bounded, reproducible, and free of real credentials or data.
- Do not document bypass, evasion, persistence, or collection techniques beyond
  what the project implements for explicitly authorized assessments.
- Never include real targets, tracking identifiers, browser profiles, session
  material, personal information, tokens, secrets, or production logs.
- Update related pages when a change affects more than one workflow or
  configuration surface.
- Add redirects in `docs.json` when moving an already published page.

## Pull requests

Describe the user problem, the source material checked, the pages changed, and
the validation performed. Link the corresponding P-BitM issue or pull request
when documenting a product change. Include screenshots for meaningful visual
or navigation changes, but redact all sensitive information.

## Licensing and third-party material

P-BitM's original documentation is licensed under the GNU General Public
License version 3 only (`GPL-3.0-only`). By submitting a contribution, you
confirm that you have the right to provide it and agree that it will be
distributed under the license applicable to the files you modify.

Do not submit copied text, images, diagrams, or code from unlicensed or
incompatible sources. Identify the upstream project, canonical URL, affected
files, relationship, copyright notice, and license whenever third-party
material is incorporated or adapted. Update
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) when required.

## Security and conduct

Do not disclose a suspected vulnerability in a public issue or pull request.
Follow [SECURITY.md](SECURITY.md). All participation is governed by
[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
