# Domain Docs

## Before exploring, read these

- `GLOSSARY.md` at the repo root, or `GLOSSARY-MAP.md` if it exists; read relevant context glossaries it points to.
- `docs/adr/` for decisions that touch the area. In multi-context repos, also check `src/<context>/docs/adr/`.

If these files don't exist, proceed silently. The domain-modeling skill creates them when terms or decisions are resolved.

## File structure

This is a single-context repo:

- `GLOSSARY.md` at the root
- ADRs in `docs/adr/`

## Use the glossary's vocabulary

Use defined domain terms in issues, refactor proposals, hypotheses, and test names. If a needed concept is missing, reconsider whether it is invented or note the gap for domain-modeling.

## Flag ADR conflicts

Surface contradictions with existing ADRs rather than silently overriding them.
