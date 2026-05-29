# Commit message guide

Write a Git commit message following these rules:
1. Start with a summary line (max 50 characters)
2. Leave a blank line after the summary
3. Add a detailed description with lines wrapped at 72 characters
4. Use imperative mood ("Add feature" not "Added feature")
5. Explain what and why, not how
6. Focus on the changes made in this commit
7. Use conventional commits

Format:

```plain
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

Types:

fix
: a commit of the type `fix` patches a bug in your codebase (this correlates
  with PATCH in Semantic Versioning).

feat
: a commit of the type `feat` introduces a new feature to the codebase.

BREAKING CHANGE
: a commit that has a footer `BREAKING CHANGE:`, or appends a ! after the
  type/scope, introduces a breaking API change. A BREAKING CHANGE can be
  part of commits of any type.

Types other than `fix:` and `feat:` are allowed. For example,
`@commitlint/config-conventional` (based on the Angular convention)
recommends `build:`, `chore:`, `ci:`, `docs:`, `style:`, `refactor:`,
`perf:`, `test:`, and others.

Footers other than `BREAKING CHANGE: <description>` may be provided and
follow a convention similar to Git trailer format.
