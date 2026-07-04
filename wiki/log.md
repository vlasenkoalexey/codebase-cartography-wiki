# Wiki log

Append-only, chronological. One entry per operation, prefixed so it stays greppable with plain Unix
tools (`grep '^## \[' wiki/log.md | tail -5`). Prefixes: `ingest-code | <slug>` (code repo via the
skill), `ingest | <source>` (article/doc/note), `connect | <scope>` (cross-repo), `lint | <scope>`,
`note | <title>`. Newest at the bottom.

## [2026-07-04] ingest-code | wikify-repo
Ingested [wikify-repo](https://github.com/vlasenkoalexey/wikify-repo) as a submodule pinned at
`05228d7` (`raw/code/wikify-repo`). Lens: code comprehension (survey comparability). Built 16 grounded
concept pages + an overview + 14 doc-concepts (from README, docs/design.md, docs/implementation.md);
48 module catalogs cover all 664 symbols (100% represented, 52.3% deep). `finalize` citation lint: OK.
Adversarial `verify`: 216 load-bearing claims across 16 pages re-checked against source — 4 pages got
small factual corrections (over-scoped "every command" claims on cli/acquire, a docstring attribution
on verify, rule-scoping + a non-frozen dataclass on lint); all others held. First silo in the survey —
no cross-repo `connect` yet (needs a 2nd tool).
