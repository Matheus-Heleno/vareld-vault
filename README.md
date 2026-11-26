# Vareld Vault

A local-first password manager focused on security, privacy, and performance.

> **Status: Experimental.** Vareld Vault is under active research and development. It is not ready for storing real passwords or other sensitive credentials.

## Overview

Vareld Vault is an experimental password manager project. Its goal is to explore a practical, privacy-oriented way to store and manage credentials locally, while evaluating implementation choices through measurable tests.

The project does not have a predefined programming language. Different languages and implementation approaches may be prototyped and compared before a final technical direction is selected.

## Project goals

- Keep the user's vault under local control.
- Minimize unnecessary collection, transmission, and exposure of sensitive data.
- Use well-reviewed cryptographic primitives and established security practices.
- Prioritize predictable behavior, maintainability, and performance.
- Document design decisions, limitations, and test results.

## Current development principles

- **Local-first:** local storage is the intended default; cloud synchronization is not assumed.
- **Security before convenience:** cryptographic design and threat modeling must precede real-world use.
- **Evidence-based engineering:** language and architecture choices should be supported by benchmarks and testing.
- **Transparency:** implemented features, experiments, and planned work must be clearly distinguished.

## Documentation

- [Product overview](docs/PRODUCT.md)
- [Architecture and technical direction](docs/ARCHITECTURE.md)
- [Security model](docs/SECURITY.md)
- [Benchmarks and language evaluation](docs/BENCHMARKS.md)
- [Roadmap](docs/ROADMAP.md)

## Important security notice

This repository describes an experimental project, not a security-audited password manager. Do not use it to store real credentials, recovery codes, financial information, or other sensitive data. Security mechanisms described in the documentation are design considerations unless explicitly identified as implemented and tested.

## Development

The implementation language and final technology stack have not been selected. Prototypes may be developed in different languages to compare performance, security properties, ecosystem maturity, and maintainability.

No production installation or usage instructions are provided while the project remains experimental.

## License

No license has been selected yet. Unless a license is added to this repository, all rights are reserved by the copyright holder.
