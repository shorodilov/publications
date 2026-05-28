AI Guidelines
===

This repository is a working archive for publications. It stores original
authorial publications and permitted adaptations of third-party publications,
such as translations, annotations, or derivative works. It is not a generic
archive of third-party materials.

Repository Structure
---

- Use `README.md` as the source of truth for repository structure.
- Each publication is stored as a separate unit under `src/<pub-id>`.
- `src/<pub-id>/index.*` is the publication entry-point or master file.
- `index.*` may contain the full text directly or assemble section files such
  as `section/xx-sectiontitle.*`.
- `.ai/` directories may contain publication-specific AI instructions. Follow
  them when working inside that publication.

Metadata
---

- `src/metadata.yaml` contains shared metadata used as defaults for all
  publications.
- `src/<pub-id>/metadata.yaml` contains publication-specific metadata.
- When the same key exists in both files, `src/<pub-id>/metadata.yaml`
  overrides `src/metadata.yaml`.
- Do not remove license, source, author, date, or attribution metadata unless
  explicitly asked and the reason is clear.
- Preserve existing metadata structure unless a requested change requires a
  schema-compatible update.

Pandoc Schema
---

- `src/metadata.schema.json` defines the current metadata schema.
- The schema is currently Pandoc-oriented.
- Check metadata changes against the schema before adding new fields or changing
  value shapes.
- Structured `author` objects may require custom Pandoc templates; do not assume
  every Pandoc output format will render them correctly without template support.

Authored Publications
---

- Treat authorial text as source material.
- Do not rewrite authorial text unless explicitly asked.
- Preserve the author's voice, language, terminology, spelling conventions, and
  argument structure.
- For Ukrainian publications, keep Ukrainian text in Ukrainian unless
  translation is requested.
- Limit edits to the requested scope: typo fixes, metadata updates, structure
  cleanup, or other clearly requested changes.

Adaptations and Attribution
---

- Store third-party material as a publication only when it is being adapted and
  the original license permits the adaptation.
- Preserve attribution to the original author and source.
- Preserve license notices, source links, translator or adapter notes, and other
  provenance metadata.
- Do not imply that adapted third-party work is original authorial work.
- If license compatibility or attribution is unclear, flag the uncertainty
  instead of removing or weakening attribution.

AI Editing Rules
---

- Prefer small, reviewable changes.
- Do not make broad style rewrites, tone changes, or language normalization
  without explicit instruction.
- Do not invent build commands, scripts, CI, workflow files, or publication
  pipelines.
- Do not modify `README.md` or `src/metadata.schema.json` unless fixing a clear
  typo or a direct contradiction with requested guidance.
- When preparing prompts or replacement text, provide complete text from start
  to finish, not partial "insert this here" fragments.
- Keep unrelated files unchanged.

Expected Change Style
---

- Keep repository guidance concise and operational.
- Use Markdown for prose documents.
- Match existing heading style in repository guidance files.
- Prefer direct bullets over generic policy language.
- Explain any metadata, attribution, or license-sensitive change in the final
  summary.
