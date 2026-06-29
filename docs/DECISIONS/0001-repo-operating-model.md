# 0001: Public Repo Operating Model

Date: 2026-06-29

## Decision

Use a public GitHub repository for safe coordination, task split, PR review, and public-ready implementation only.

Private or unreviewed material stays outside the public repository.

## Rationale

The project will involve market research, generated assets, commercial tools, and Steam release data. A public repository is useful for veripsa core, PR review, and task tracking, but it must not become a dump for raw research media, secrets, or unlicensed assets.

## Consequences

- Every asset needs source/license notes before entering the public repo.
- PRs must include public safety checks.
- Branch protection is required on `main`.
- Rejected generated work is preserved privately unless approved for public release.

