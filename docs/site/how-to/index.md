# How-to guides

Task recipes. Each assumes sibling checkouts of this repo and of the platform
repos it patches.

## Add a token kind

Add a `LexerRuleDef` fragment with a `priority` below the catch-all rules; no Rust change is needed.

## Debug a tokenization surprise

Dump the collected rules sorted by priority — most surprises are an ordering tie, not a missing rule.
