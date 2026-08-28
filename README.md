# P-BitM documentation

This repository contains the product documentation for
[P-BitM](https://github.com/P-BitM-Framework/P-BitM), a containerized platform
for controlled browser-in-the-middle security assessments.

> [!CAUTION]
> Use P-BitM only on systems you own or where you have explicit written
> authorization.

## Local preview

The documentation CLI requires Node.js 20.17.0 or newer. Install the current CLI,
then start the preview from this repository root:

```bash
npm install --global mint
mint dev
```

Open `http://localhost:3000`.

Before opening a pull request, run:

```bash
mint validate
mint broken-links --check-anchors
mint a11y
git diff --check
```

## Repository layout

- `docs.json` defines the documentation theme, navigation, and site-wide links.
- `index.mdx` is the documentation landing page.
- Topic directories contain the published MDX pages.
- `assets/` contains documentation-owned images and video demos.
- `.github/` contains contribution templates and ownership rules.

The P-BitM implementation and its checked-in runtime contracts remain the
authoritative source for product behavior. Documentation changes that describe
new or changed behavior should reference the corresponding P-BitM change.

Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting changes.

## License

Unless otherwise annotated by a lower-level license or file-level notice,
original files in this repository are distributed under the GNU General Public
License version 3 only (`GPL-3.0-only`). See [LICENSE](LICENSE) and
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
