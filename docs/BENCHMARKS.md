# Benchmarks and Language Evaluation

## 1. Purpose

The project has no predefined programming language. This document defines how implementation candidates should be compared before choosing a long-term direction.

## 2. Evaluation criteria

Each prototype should be evaluated across:

| Area | What to measure |
| --- | --- |
| Startup | Time from launch to ready state |
| Unlock | Time required for the key-derivation and unlock workflow |
| Encryption | Time to encrypt representative vault payloads |
| Decryption | Time to decrypt representative vault payloads |
| Search | Time to search small, medium, and large datasets |
| Memory | Idle and peak memory usage |
| Binary size | Size of the distributable build |
| Reliability | Test results, crashes, and error handling |
| Ecosystem | Cryptographic library maturity and maintenance |
| Maintainability | Code clarity, tooling, and development complexity |

## 3. Fair testing rules

- Use the same hardware and operating system for comparable runs.
- Record compiler/interpreter versions, build mode, and dependency versions.
- Separate debug and release measurements.
- Use identical input datasets and equivalent algorithms.
- Run multiple iterations and report median and spread, not only the best result.
- Distinguish cold-start from warm-start measurements.
- Do not weaken cryptographic parameters to make a candidate appear faster.
- Keep benchmark data synthetic; never use real credentials.

## 4. Security is a constraint

Performance is not the only selection criterion. A candidate with faster execution should not be preferred if it requires immature cryptographic dependencies, unsafe memory handling, or substantially greater implementation risk.

## 5. Results

No verified comparative benchmark results are published yet. Results should be added only after the methodology is reproducible and the measurements have been collected.

Suggested result format:

| Candidate | Test environment | Startup | Unlock | Memory | Notes |
| --- | --- | ---: | ---: | ---: | --- |
| Pending | Pending | — | — | — | No verified result |

## 6. Final decision

The language decision will be documented after prototypes have been evaluated. Until then, the project remains language-agnostic.
