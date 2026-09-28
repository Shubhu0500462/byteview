# byteview

Fast line/byte counter written in Rust

## Install

```bash
cargo build --release
```

## Usage

```bash
./target/release/byteview src/*.rs
cat README.md | ./target/release/byteview
```

## Features

- Counts lines, words and bytes like wc
- Zero dependencies outside std
- Reads stdin or multiple files
- Parallel over files with std threads

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   └── main.rs
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
└── Cargo.toml
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.
