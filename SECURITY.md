# Security Policy

This repository is a public GitHub workflow lab. It must not contain production code, customer data, credentials, tokens or private keys.

## Reporting a security issue

If you notice a sensitive file or unsafe example, open a private channel with the repository owner instead of publishing the secret in an issue or pull request.

## Files that must not be committed

- `.env` or environment-specific variants.
- Private keys such as `.pem`, `.key` or `id_rsa`.
- Service account files.
- Tokens, credentials or exported secrets.

## Maintainer checklist

- Review every diff before merge.
- Keep `.gitignore` updated for common secret file names.
- Prefer small pull requests with clear scope.
