## Description

[A clear and concise description of the PR]

## Type of Change
- [ ] `feat:` New feature (adds non-breaking functionality)
- [ ] `fix:` Bug fix (non-breaking change resolving an issue)
- [ ] `docs:` Documentation updates
- [ ] `refactor:` Code changes that neither fix a bug nor add a feature
- [ ] `chore:` Dependencies, CI/CD, build tools or version updates

## Scope Impacted
- [ ] `backend` (Axum core, sqlx, migrations)
- [ ] `frontend` (Routing, UI elements)
- [ ] `shared` (Shared types, configurations)
- [ ] `lukko` (Authentication module)
- [ ] `vintti` (Knowledge vault module)
- [ ] `henki` (CRM module)
- [ ] `aihe` (Chat module)
- [ ] `keruu` (Forms module)

## Checklist

### Code quality
- [ ] **Testing:** Unit or integration tests have been added/updated to cover these changes.
- [ ] **Local Verification:** All tests pass locally (`cargo test` / `pnpm test`).
- [ ] **Lint & Format:** Code is cleanly formatted and passes static analysis (`cargo clippy`, `cargo fmt`, `pnpm lint`).
- [ ] **Clean Code:** Removed all temporary `println!`, `console.log`, or commented-out code blocks.

### Documentation
- [ ] **Code Comments:** Complex cryptographic logic, database queries, or non-obvious code paths are clearly commented inline.
- [ ] **External Docs:** Updated the root `README.md`, architecture guides, or module documentation if this alters public interfaces or configuration steps.

### Security
- [ ] **Zero-knowledge:** Verified that no unencrypted data or sensitive metadata is transmitted or logged to the server
- [ ] **State isolation:** Cryptographic keys are managed purely in active
  memory threads / Web Workers and are zeroed out appropriately
- [ ] **Audit trail:** If this change mutates state, a corresponding signed
  receipt is pushed to the `audit_ledger`

## 🔗 Backlog Linkage
Closes #---

## 📝 Squash-Commit Body Documentation
