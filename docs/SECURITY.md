# Security Policy

## Supported scope

This repository primarily contains publication materials, metadata
schemas, examples, and supporting documentation.

The supported security scope is the current default branch and the latest
published repository state. Older branches, experiments, drafts, and local
work-in-progress files are not supported unless maintainers explicitly say
otherwise.

## What counts as a security issue

Please report security-sensitive problems such as:

- Exposed secrets, tokens, credentials, or private URLs.
- Unsafe publication or build instructions that could lead to command
  injection, arbitrary file access, or unintended network access.
- Malicious links or embedded content in examples or documentation.
- A dependency or workflow issue that can compromise contributors or
  generated artifacts.
- Any issue that should not be disclosed publicly before maintainers have
  a chance to review it.

Normal typos, broken links, schema validation bugs, formatting problems,
and content disagreements are not security issues. Use regular issues or
pull requests for those.

## Reporting a vulnerability

Do not open a public issue with sensitive details.

Preferred reporting path:

1. Use GitHub private vulnerability reporting if it is enabled for this
   repository.
2. If private vulnerability reporting is not enabled, contact the
   maintainers through a private channel listed in the repository or
   organization profile.
3. If no private contact is available, open a minimal public issue asking
   maintainers to provide a private security contact. Do not include
   exploit details, secrets, or reproduction steps in that public issue.

Include the following information when possible:

- A short description of the problem.
- The affected file, workflow, dependency, or generated artifact.
- Steps to reproduce, if safe to share privately.
- The potential impact.
- Whether the issue is already public.

## Response expectations

Maintainers will make a best effort to acknowledge valid reports, assess
impact, prepare a fix when needed, and coordinate disclosure.

This is a small repository, so response times may vary. Please avoid
public disclosure until maintainers have had a reasonable opportunity to
review the report.

## Disclosure

After a fix is prepared, maintainers may publish a security advisory,
release note, changelog entry, or public issue summary depending on the
severity and repository impact.

Reports made in good faith are appreciated.
