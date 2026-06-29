# Security Policy

## Do Not Commit

- API keys, tokens, cookies, credentials, signing certificates, or license keys.
- Steam partner IDs, depot IDs, unpublished build data, revenue data, or contract material.
- Paid API prompts, paid generation outputs, or tool account data unless a separate public release decision exists.
- Unverified third-party assets, reference images, music, video, fonts, or ripped media.

## Reporting

Open a private security report or contact the repository owner directly. Do not paste secrets into public issues or pull requests.

## Required Checks

The repository is expected to run:

- `repo-policy / validate`
- `secret-scan / gitleaks`

Branch protection should require review, conversation resolution, and passing checks before merging into `main`.

