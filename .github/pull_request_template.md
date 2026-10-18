## What and why

<!-- What this changes, and the problem it solves. Link the issue if there is one. -->

## Checklist

- [ ] Tests cover the change (and fail without it)
- [ ] Per-frame code still allocates nothing (`tests/zero_alloc.rs`)
- [ ] `cargo clippy --workspace --all-targets -- -D warnings` and `cargo fmt --check` pass
- [ ] Documentation updated (rustdoc, README, examples)
