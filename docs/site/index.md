# engine-lex-pattern

The data-driven lexer: every pattern comes from the language definition.

## What it is

A lexer engine with **no Rust lexing logic**. It collects `LexerRuleDef`
fragments from the `Language`, sorts them by `priority` ascending, and applies
them: literals, character classes, numbers and delimited blocks are all data.
Swapping the lexer is a change to `lexer_rules`, not a recompile (ADR-0044
§1, §3).

## Start here

- **Reference** — [public API](/engine-lex-pattern/reference/)
- **How-to** — [task recipes](/engine-lex-pattern/how-to/)
- **Explanation** — [design and rationale](/engine-lex-pattern/explanation/)

No tutorials: this repo is a building block used from Rust. End-to-end
walkthroughs live with the product that composes it — see the
[Handl platform](/handl/).
