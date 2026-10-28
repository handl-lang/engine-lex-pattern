# engine-lex-pattern

`hnl-engine-lex-pattern` — A **data-driven** lexer engine that reads [`LexerRuleDef`] fragments from a [`Language`] and tokenizes source text (ADR-0044 §1, §3).

## Development

```bash
cargo fmt --check && cargo clippy --all-targets -- -D warnings && cargo test
```

`ci.sh` is the gate (fmt → clippy → test → doc). Deps resolve from git, so no
sibling checkouts are needed; a plain clone test-runs as-is.

## License

MIT.

## Documentation

Published site (Diátaxis): <https://handl-lang.github.io/docs/engine-lex-pattern/>

- [Reference](https://handl-lang.github.io/docs/engine-lex-pattern/reference/) — public API surface
- [How-to](https://handl-lang.github.io/docs/engine-lex-pattern/how-to/) — task recipes
- [Explanation](https://handl-lang.github.io/docs/engine-lex-pattern/explanation/) — design and rationale

Decision records live on the `project` branch under `project/adrs/`.
