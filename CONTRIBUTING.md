# Contributing to densa

Thank you for helping. Issues, ideas and pull requests are welcome in every densa-rs
repository.

## Before you start

- **Bugs:** open an issue with what you did, what you expected and what happened, your OS,
  GPU and Rust version.
- **Larger changes** (a new crate, a public API, a new dependency): open an issue first so
  the design can be agreed before the code is written.
- **Security issues:** do not open a public issue; see [SECURITY.md](SECURITY.md).

## Pull requests

1. Keep a pull request to one change, with tests.
2. Run the checks the repository lists under "Development" in its README (tests, Clippy with
   `-D warnings`, rustfmt, docs, the minimum Rust version).
3. Write commit messages as `type: description` (`feat`, `fix`, `refactor`, `docs`, `test`,
   `chore`, `perf`, `ci`).
4. Update the documentation that your change affects: rustdoc, the README, examples.

## What densa expects of code

- **Frames do not allocate.** Code on a per-frame path (drawing, scrolling, hit-testing,
  reading a view) must not allocate; prove it with a test using `densa-alloc`'s counting
  allocator, as the existing `tests/zero_alloc.rs` files do.
- **Tests must catch bugs.** A test that still passes when the code under it is deliberately
  broken is not testing it. Prefer tests that check behavior against a simple model.
- **Every `unsafe` block** carries a `// SAFETY:` comment, and every atomic operation a
  comment justifying its ordering.
- **No panics on public input.** Return an error for anything a caller can get wrong.
- **English** in code, comments, documentation and examples.

By contributing, you agree that your contributions are dual-licensed under MIT or
Apache-2.0, as the projects are.
