# Vareld Vault

A local-first password manager focused on security, privacy, and performance.

> **Status: Experimental.** Vareld Vault is under active research and development. It is not ready for storing real passwords or other sensitive credentials.

## Overview

Vareld Vault is a long-term software project with the ambition to become a reliable, highly secure, privacy-focused password manager that anyone can use. It is not intended to remain only a personal project: the goal is to develop it into a public product, make it available to the wider community, and build it with real users and contributors in mind.

This is a large undertaking. A password manager must protect some of the most sensitive information a person owns, so the project will prioritize careful engineering, extensive testing, transparent security practices, and independent review where possible. The ambition is to reach a high standard of security, but no software can honestly promise to be completely secure; security claims must be supported by evidence.

When Vareld Vault is ready for public release, the intention is for people to be able to use it, not just to serve as a private tool for its creator. The project will remain experimental until its core functionality and security have been properly developed and evaluated.

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
- **Community-oriented:** build toward a public release that can serve users beyond the project's creator.

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

Vareld Vault is licensed under the [MIT License](LICENSE). You are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, subject to the conditions stated in the license.

Copyright (c) 2026 Matheus H.
