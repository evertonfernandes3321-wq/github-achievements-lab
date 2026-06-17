# Secret Check Guide

Public repositories should never receive credentials, private keys or local environment files.

## File names to inspect

Look carefully for:

- `.env`
- `.env.local`
- `.env.production`
- `*.pem`
- `*.key`
- `id_rsa`
- `credentials.json`
- `service-account.json`
- `secrets.*`
- `token*`
- `private*`

## Before committing

Run a local file-name scan and inspect the staged diff:

```powershell
git status --short
git diff --cached --stat
```

If a sensitive file appears, stop and remove it from the commit before pushing.
