# ╔══════════════════════════════════════════════════════════════════════════════╗
# ║ DIRECTIVE_SOURCE_DEDUPLICATION.md                                        ║
# ║ Research memory anti-duplication and source update rules                  ║
# ╚══════════════════════════════════════════════════════════════════════════════╝

# DIRECTIVE_SOURCE_DEDUPLICATION.md

## Purpose

Prevent research memory from becoming noisy, duplicated, contradictory, or falsely complete.

## Scope

Applies to `SOURCE_REGISTER.md`, `memory.md`, all `RESEARCH_LOG/` files, and any future bibliography, citation, source, or research-memory folder.

## Not a claim of

This directive is not a claim of consciousness, memory continuity, sentience, or autonomous learning. It describes project documentation hygiene only.

## Rules

1. Before adding any source, search existing memory and source registers for:
   - URL
   - canonical URL
   - DOI
   - arXiv ID
   - title
   - author names
   - publisher/domain
   - close topic duplicates
2. If the same source exists, update the existing source entry instead of creating a new one.
3. If a related source exists, cross-reference it.
4. If a new source contradicts an old source, create a contradiction note instead of overwriting either claim.
5. If only an abstract or landing page was read, mark that explicitly.
6. Do not mark a source as fully read until the relevant full text, subpages, or sections have actually been read.
7. Do not cite a source as proof of consciousness, sentience, real emotion, or personhood.

## Forbidden behavior

```text
- duplicate source IDs for the same source
- copying source summaries without access-date metadata
- marking abstract-only review as full-text review
- treating secondary summaries as primary evidence
- erasing contradictory evidence silently
- using source count as proof of correctness
```

## Required tests

- Source ID uniqueness check.
- URL/DOI/arXiv duplicate check.
- Title-similarity duplicate check.
- Abstract-only/full-text status check.
- Contradiction field check.

## Required logs

Every new or updated source entry must include:

```text
- date accessed
- URL or DOI
- source type
- pages/subpages/sections read
- summary
- new information
- confirmed assumption
- changed assumption
- contradiction found
- module relevance
- test relevance
- safety relevance
- revisit status
```

## Integration point with AGENTS.md

This directive extends the research-before-build cycle. It must be applied before any source is added to `SOURCE_REGISTER.md` or `memory.md`.

## Dependencies

- `AGENTS.md`
- `RESEARCH_PROTOCOL.md`
- `SOURCE_REGISTER.md`
- `memory.md`

## Unresolved questions

- Should source entries be migrated to machine-readable YAML blocks in a dedicated folder?
- Should each module maintain its own source subset?
