# linely

Learning Rust by rewriting coreutils, one tool at a time

Small but I use it weekly.

## Getting started

```bash
cargo build --release
```

## What it does

- Reads stdin or multiple files
- Zero dependencies outside std
- Parallel over files with std threads
- Counts lines, words and bytes like wc

## Examples

```bash
./target/release/linely src/*.rs
cat README.md | ./target/release/linely
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── faq.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── Cargo.toml
├── LICENSE
└── Makefile
```

## Development

```bash
cargo test
cargo clippy -- -D warnings
```

## Development

```bash
# run the test suite
pytest -q   # or npm test / go test ./...
```

## License

MIT licensed, see LICENSE.
