# Documentation style guide

## Audience and voice

Write for security practitioners and maintainers who may be new to P-BitM but
understand Docker and basic web infrastructure. Use direct, concise sentences,
present tense, and active voice. State prerequisites before actions and explain
the consequence of destructive commands.

Use **operator** for an authorized dashboard user, **participant** for a
campaign session or stored campaign record, and **authorized assessment
target** when discussing the person who opens a campaign link. Use **victim**
only when matching an existing API, CLI, database, or code identifier.

## Page structure

Every published page must begin with:

```yaml
---
title: "Clear page title"
description: "One sentence explaining the page outcome."
---
```

Start with the purpose or outcome. Use sentence case for headings. Keep each
page focused on one task or concept and link to detailed references instead of
duplicating them.

## Documentation components

Use components only when they improve scanning:

- `<Steps>` for ordered procedures;
- `<Warning>` for safety, destructive actions, or data-loss risks;
- `<Note>` for context that affects understanding;
- `<Tip>` for optional shortcuts or operational advice;
- `<Card>` and `<Columns>` for navigation from overview pages.

Do not hide essential instructions in accordions or tabs.

## Commands and configuration

Use fenced code blocks with a language. Commands must be copied from or checked
against the current P-BitM CLI. Use placeholders such as `<campaign-id>` and
`example.com`; never use real infrastructure, tokens, or personal data.

Describe defaults as defaults, not guarantees. Name the source file or
configuration key when behavior depends on configuration.

## Links and assets

Use root-relative links for this documentation, for example
`[Quick start](/getting-started/quick-start)`. Use canonical HTTPS URLs for
external sources. Provide useful alt text for every informative image and do
not place sensitive data in screenshots or image metadata.

## Review checklist

Confirm that the page is accurate against P-BitM, scoped to authorized use,
free of secrets and personal data, present in `docs.json`, linked correctly,
and readable in both light and dark mode.
