# Explanation

## Why this crate exists

Hand-written lexers put grammar knowledge in Rust, so every language variant
needs a fork. Reading the rules from data keeps one engine for all languages and
makes grammar reviewable as data.

## Where it sits

This crate belongs to the `engine-*` family. Plugins, kits and hosts reach it
through the kit's operation slot, so the engine can be swapped without touching a
language definition.

See the [reference](/engine-lex-pattern/reference/) for the API and the
[how-to guides](/engine-lex-pattern/how-to/) for tasks.
