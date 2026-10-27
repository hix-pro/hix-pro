![hix tools](./banner.svg)

**Local-first developer tools that catch what CI misses.** Everything in this suite runs on your machine or in your own CI: no backend, no account, and no data leaving your environment. Each tool does one review job well — and each one ships the machine-readable output and exit codes you need to gate a pipeline on it.

## Tools

| Tool | What it catches | Language |
| --- | --- | --- |
| [EnvAudit](https://github.com/hix-pro/env-audit) | environment variables that are missing, undocumented, or unused | Rust |
| [Migration Guard](https://github.com/hix-pro/migration-guard) | dangerous SQL migrations, before they run | Rust |
| [API Watch](https://github.com/hix-pro/api-watch) | breaking changes in OpenAPI and JSON contracts | Rust |
| [ActionLens](https://github.com/hix-pro/action-lens) | what a GitHub Actions workflow really does | TypeScript |
| [ComposeMap](https://github.com/hix-pro/compose-map) | production red flags in Docker Compose stacks | TypeScript |
| [TypeShift](https://github.com/hix-pro/typeshift) | the semver bump your TypeScript release implies | TypeScript |
| [RepoRace](https://github.com/hix-pro/reporace) | which GitHub repositories are accelerating | TypeScript |
| [OpenCode Telegram](https://github.com/hix-pro/opencode-telegram) | your local OpenCode agent, remote-controlled | Python |

## Principles

- **Local-first** — your code and data never leave your machine. Tools that parse untrusted input treat every file as hostile.
- **No backend** — everything runs in the CLI, the browser, or your CI. No accounts, no telemetry, no phone-home.
- **CI-ready** — JSON output modes, documented exit codes, and GitHub Action wrappers so findings block merges, not just scroll by.

## Getting started

Every repo has a quick start at the top of its README. The Rust CLIs install with `cargo install`, the browser tools run from a deployed demo or locally with `npm run dev`, and the Telegram bridge sets up with one config file and a systemd unit. Check a repo's `examples/` or fixtures when you want to see the rules fire on real input.

## Contact

Found a bug or want a feature? Open an issue on the relevant tool. Security reports go through each repo's **Security** tab — see its [SECURITY.md](https://github.com/hix-pro/env-audit/blob/main/SECURITY.md) for the process and response timeline.
