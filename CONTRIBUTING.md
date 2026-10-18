# Contributing

Thank you for helping improve these tools. This guide applies to every repository in the organisation unless a repository has its own.

## Before you start

- **Questions and ideas:** open an issue first for anything beyond a small fix, so we can agree on the direction before you write code.
- **Security problems:** do not open an issue. See [SECURITY](SECURITY.md).
- **Scope:** these repositories contain client tooling. They do not contain the ZenXPAM platform, and we cannot accept changes that depend on platform internals.

## How to contribute

1. Fork the repository and create a branch from `main`.
2. Make a focused change, with tests where the repository has them.
3. Run the repository's tests and linters using the commands in its README. A change that breaks them cannot be merged.
4. Update documentation and examples for any behaviour you change.
5. Commit with a clear message and **sign off** each commit (see below).
6. Open a pull request that explains what changed and why, and links the issue it addresses.

## Developer Certificate of Origin

We use the [Developer Certificate of Origin](https://developercertificate.org/) instead of a separate contributor agreement. By signing off a commit, you confirm that you wrote it or have the right to submit it under the repository's licence.

Sign off with:

```bash
git commit -s -m "Describe the change"
```

This adds a `Signed-off-by: Your Name <you@example.com>` line.

## Code standards

- Keep changes small and readable. Match the style of the surrounding code.
- **Never log, print or commit secrets**, even in tests. Use clearly fake values in test fixtures, and keep them obviously fake (for example a `KEYMARKER` placeholder).
- Prefer the standard library where the repository already does so (`zenx-secret` uses only the Go standard library, and a change that adds a dependency needs a strong reason).
- Write error messages that help the user fix the problem without revealing sensitive values.
- Keep behaviour backward compatible within a major version, and call out any breaking change in the pull request.

## Review

A maintainer from the Zenxsys team will review your pull request, usually within a week. We may ask for changes. We aim to be respectful and clear, and we ask the same of you; see the [Code of Conduct](CODE_OF_CONDUCT.md).

## Licence

These repositories are released under the **Apache License 2.0**. By contributing, you agree that your contribution is licensed under the repository's licence (see its `LICENSE` file).
