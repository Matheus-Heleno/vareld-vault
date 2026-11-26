# Roadmap

This roadmap describes intended research and development stages. It is not a promise that every item is implemented or scheduled.

## Phase 1 — Research and foundations

- [x] Establish project identity and initial documentation.
- [x] Define language-agnostic evaluation criteria.
- [ ] Compare implementation language candidates.
- [ ] Research cryptographic library options.
- [ ] Draft a detailed threat model.
- [ ] Record initial architecture decisions.

## Phase 2 — Technical prototypes

- [ ] Build minimal prototypes in selected candidate languages.
- [ ] Test local encrypted storage.
- [ ] Evaluate key derivation and authenticated encryption workflows.
- [ ] Compare startup, memory, and operation performance.
- [ ] Add automated tests for core primitives and data handling.

## Phase 3 — Core application

- [ ] Select and document the primary technology stack.
- [ ] Implement vault creation and unlock.
- [ ] Implement credential entry management.
- [ ] Implement password generation.
- [ ] Implement locking and sensitive-data handling.
- [ ] Define backup, restore, and file-format migration behavior.

## Phase 4 — Hardening

- [ ] Expand security and regression testing.
- [ ] Review dependencies and build pipeline.
- [ ] Test corrupted and maliciously modified vault files.
- [ ] Review memory, clipboard, logging, and temporary-file exposure.
- [ ] Arrange independent security review before any production claims.

## Phase 5 — Release preparation

- [ ] Define supported platforms.
- [ ] Prepare packaging and update procedures.
- [ ] Publish user documentation and known limitations.
- [ ] Establish a responsible vulnerability disclosure process.
- [ ] Decide whether the project is ready for a public beta.

## Current stage

The project is in the research and prototype stage. The language, final architecture, and production feature set remain undecided.
