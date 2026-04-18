# Awesome AI-Friendly CLI

> Flags and configs to silence CLI noise for AI agents. Save 60-90% of wasted tokens.

AI agents don't need progress bars, color codes, banners, or interactive prompts. Most CLI tools have flags to turn these off — but they're buried in docs and scattered across ecosystems. This repo collects them in one place.

## Contents

- [Ecosystems](#ecosystems)
- [Common Patterns](#common-patterns)
- [Tools](#tools)

## Ecosystems

- [Node.js](node.md) - npm, npx, yarn, pnpm, eslint, prettier, biome, jest, vitest, mocha, tsc, playwright, cypress
- [Python](python.md) - pip, uv, poetry, pytest, ruff, mypy, pyright, black, flake8, pylint, isort, bandit, coverage, tox, django, flask
- [PHP](php.md) - php-cs-fixer, phpcs, phpstan, psalm, phpunit, pest
- [Go](go.md) - go build, go test, go vet, go mod, golangci-lint, staticcheck, gofmt, goimports, govulncheck
- [Rust](rust.md) - cargo build, cargo check, cargo test, cargo clippy, cargo fmt, cargo-nextest, cargo-audit, cargo-deny
- [Ruby](ruby.md) - bundler, rake, rspec, minitest, rails test, rubocop, standard, sorbet, reek, brakeman, erb_lint
- [Java](java.md) - maven, gradle, javac, checkstyle, pmd, spotbugs, google-java-format, spotless
- [Kotlin](kotlin.md) - gradle, kotlinc, ktlint, detekt, spotless
- [Swift](swift.md) - swift build, swift test, xcodebuild, xcbeautify, xcpretty, swiftlint, swiftformat, swift-format, periphery
- [.NET](dotnet.md) - dotnet build, dotnet test, dotnet publish, dotnet pack, dotnet restore, dotnet format, dotnet-ef, coverlet

## Common Patterns

Most CLI tools respect some combination of:

| Flag / Env          | What it does                                                             |
|---------------------|--------------------------------------------------------------------------|
| `--no-progress`     | Disables progress bars                                                   |
| `--no-color`        | Disables ANSI color codes                                                |
| `--quiet` / `-q`    | Minimal output                                                           |
| `--json`            | Machine-readable output                                                  |
| `--non-interactive` | Disables prompts and confirmations                                       |
| `NO_COLOR=1`        | Standard env var to disable color ([no-color.org](https://no-color.org)) |
| `CI=true`           | Many tools auto-quiet when they detect CI                                |

## Tools

- [rtk](https://github.com/rtk-ai/rtk) - CLI proxy that sits between AI agents and the shell, compressing output before it reaches the LLM context window. Works with Claude Code, Gemini CLI, and OpenCode.

## Contributing

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

- [MeterCall](https://metercall.ai/?v=a&src=github) — One metered API gateway. 21M+ endpoints (payments, SMS, AI, CRMs, gov data). Free tier; pay per call.
