# Contributing Guide

Thank you for considering a contribution.

This repository is used to prepare and maintain publication materials,
metadata schemas, examples, and supporting documentation. Contributions
should make the repository easier to understand, review, reproduce, or
publish.

## Scope

Useful contributions include:

- Fixing typos, broken links, formatting issues, or unclear wording.
- Improving article drafts, examples, metadata, or repository docs.
- Updating JSON schemas and related validation examples.
- Adding missing explanations for repository workflows.
- Reporting issues with build, conversion, validation, or publication
  tooling.
- Proposing small, well-scoped improvements.

Out of scope:

- Broad rewrites without a concrete goal.
- Unrelated tooling or infrastructure changes.
- Promotional content.
- Large conceptual changes without prior discussion.

For large changes, open an issue first and describe the intent before
preparing a pull request.

## Before you start

Please check:

1. Existing issues and pull requests, to avoid duplicate work.
2. The README, to understand the repository purpose and structure.
3. Relevant schemas, examples, or article files touched by your change.
4. The license terms. Unless stated otherwise, contributions are expected
   to be compatible with the repository license.

## Repository conventions

Keep changes small and reviewable.

Prefer one pull request per topic:

- One documentation fix.
- One schema change.
- One article update.
- One repository-maintenance change.

Avoid mixing unrelated content and tooling changes in the same pull
request.

## Documentation style

When editing documentation:

- Use clear, direct language.
- Prefer practical explanations over abstract wording.
- Keep examples close to the rule or concept they explain.
- Preserve intentional terminology used by the project.
- Avoid unnecessary formatting churn.
- Do not reflow entire files unless the pull request is specifically
  about formatting.

## Schema changes

When changing a schema, include enough context for reviewers to understand
why the change is needed.

A schema pull request should normally explain:

- Which field, rule, or validation behavior changed.
- Why the previous behavior was insufficient.
- Whether existing metadata files are affected.
- Which examples or tests were updated.

If a schema change is breaking, say so explicitly in the pull request.

## Issues

Use the issue templates when possible.

A good issue includes:

- A clear title.
- The affected file or section.
- The expected behavior or expected text.
- The actual behavior or current text.
- A small reproduction case, if the issue is related to validation,
  conversion, or generated output.

Do not use public issues to report sensitive security problems. See
`SECURITY.md` instead.

## Pull requests

A good pull request includes:

- A short explanation of what changed.
- The reason for the change.
- Links to related issues, if any.
- Notes about validation or review performed.
- Screenshots or rendered output when the visual result matters.

Before opening a pull request, check that:

- The change is focused.
- The affected files are intentional.
- Markdown renders correctly.
- Examples still match the documented behavior.
- Generated files are included only when the repository expects them.

## Commit messages

Use Conventional Commits for commit messages.

For commits created by an AI agent or AI-assisted tool, set the Git author
to the model or tool identity in the form `<model> <email>`, such as
`GPT-5.5 <noreply@openai.com>` or
`Copilot {model} <noreply@github.com>`.

The repository includes a separate commit-message guide in
`COMMIT_MESSAGE.md`. Follow that guide when preparing commits.

In short:

- Start with a short summary line.
- Use the imperative mood.
- Explain what changed and why.
- Keep the body wrapped at a readable width.

Examples:

```plain
docs: add community health documents
```

```plain
fix(schema): require publication title
```

```plain
chore: normalize repository metadata
```

## Review process

Maintainers may ask for changes before merging.

Review feedback is about improving the repository. Keep discussion focused
on the change, not on the person making it.

A pull request may be closed if it is inactive, out of scope, too broad,
or inconsistent with repository goals. A closed pull request can still be
useful as prior discussion for a better-scoped future change.

## Code of Conduct

All contributors are expected to follow `CODE_OF_CONDUCT.md`.
