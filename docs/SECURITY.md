# Security Model

## 1. Security status

Vareld Vault is experimental and has not been independently security audited. It must not be used to store real credentials or sensitive information.

This document defines security goals and areas of investigation. It does not certify that the current code implements them.

## 2. Security objectives

- Protect stored vault contents against unauthorized access.
- Prevent undetected modification of encrypted data.
- Protect the master secret and derived keys.
- Minimize plaintext exposure in memory, files, logs, and the clipboard.
- Fail safely when data is invalid, corrupted, or authentication fails.
- Use established cryptographic implementations rather than custom cryptographic algorithms.

## 3. Threats to consider

The threat model should consider:

- Someone obtaining a copy of the vault file.
- Offline guessing of a weak master password.
- Modification, truncation, or corruption of vault data.
- Malware or another process running under the user's account.
- Plaintext exposure through logs, crash reports, swap, temporary files, or clipboard history.
- Weak random number generation.
- Dependency compromise and supply-chain attacks.
- Lost or damaged devices and backups.

A local password manager cannot fully protect secrets from malware or an attacker who controls an unlocked device. These limitations must be communicated.

## 4. Cryptographic design under evaluation

Candidate mechanisms include:

- **Password-based key derivation:** Argon2id, with parameters selected through security guidance and realistic performance testing.
- **Authenticated encryption:** AES-256-GCM or another reviewed AEAD construction, selected after evaluating library support and implementation constraints.
- **Randomness:** operating-system cryptographically secure random number generation for salts, nonces, and generated passwords.

These are candidates, not confirmation that the project currently implements them. Parameters, key separation, nonce management, format versioning, and failure handling require explicit design and testing.

## 5. Key management requirements

The design must define:

- How the master password is processed.
- How salts and derived keys are generated and stored.
- Whether separate keys are derived for distinct purposes.
- How keys are kept in memory and released on lock.
- How password changes and recovery work.
- What happens when the user forgets the master password.

The project must not imply that a forgotten master password can be recovered unless a deliberate recovery mechanism exists.

## 6. Implementation requirements

- Use maintained cryptographic libraries.
- Never invent or implement custom encryption primitives.
- Do not log passwords, keys, or decrypted vault contents.
- Validate all serialized input and enforce size limits.
- Treat authentication failures and malformed data as errors.
- Review dependencies and keep them updated.
- Add tests for tampering, invalid input, corrupted files, and edge cases.

## 7. Responsible use

Until the project has a reviewed implementation, meaningful test coverage, and an independent security assessment appropriate to its maturity, it should be treated as a learning and research project only.

## 8. Reporting concerns

Security issues should be reported privately to the repository maintainer rather than disclosed publicly with exploit details. A dedicated security contact and disclosure process may be added as the project matures.
