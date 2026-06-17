# Reviewing Pull Requests

This guide keeps reviews in this lab small, practical and focused on safety.

## Review order

1. Read the pull request title and summary.
2. Check whether the branch name matches the change.
3. Review the full diff before looking at the rendered files.
4. Confirm that no secret-like file was added.
5. Confirm that the change fits the repository scope.

## What to look for

- Clear documentation with no exaggerated claims.
- Small diffs that can be reviewed quickly.
- Links that point to files inside the repository when possible.
- No credentials, tokens, private keys or personal data.
- No references to production systems.

## Merge guidance

Use squash merge for small documentation changes when the pull request represents one logical change. Avoid merging if the diff includes unrelated files or unclear content.
