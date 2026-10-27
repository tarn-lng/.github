# Contributing to Tarn projects

Thanks for helping! This guide applies to every repository in the `tarn-lng`
organization unless the repository has its own `CONTRIBUTING.md` (the compiler
repo [tarn](https://github.com/tarn-lng/tarn/blob/main/CONTRIBUTING.md) does, with
build and test details). Issues and pull requests are welcome in English or Spanish.

## Before you start

- Comment on the issue you want to take so a maintainer can assign it to you,
  and wait for the assignment before starting. If an assigned issue has had no
  activity for two weeks, feel free to ask whether it is still in progress.
- Issues labeled `good first issue` are a good place to start.
- Questions and ideas: [Discussions](https://github.com/tarn-lng/tarn/discussions).

## Library repositories (drivers, Flame, HTTP/2, gRPC, ...)

You need the `tarn` compiler (see the [website](https://tarn-lng.github.io/website/)
or build it from [tarn](https://github.com/tarn-lng/tarn)). Then:

```bash
tarn fetch   # downloads and hash-verifies locked packages
tarn check
tarn test
```

## Rules

- Small, focused pull requests, one topic each. Describe the behavior change and link the issue.
- Every fix ships with a test when the repository has a test suite.
- AI-assisted PRs are welcome; you must have run the tests and understand the diff.
- Packages must never gain install/build hooks.
- Language or semantics changes are discussed in the `tarn` repo first (ADRs live in `docs/adr/`).

## Code of conduct

All projects follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

Unless you explicitly state otherwise, any contribution you intentionally submit
is dual-licensed under the MIT and Apache-2.0 licenses, without any additional
terms or conditions.
