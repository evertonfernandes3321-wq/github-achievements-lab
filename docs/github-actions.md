# GitHub Actions Guide

This lab uses a small GitHub Actions workflow to verify that required documentation files exist.

## Current workflow

The `Docs Check` workflow runs on:

- pull requests;
- pushes to `main`.

It checks for required files such as `README.md`, `CONTRIBUTING.md`, `SECURITY.md` and related guides.

## Maintenance rules

- Keep workflows small and readable.
- Avoid secrets unless a workflow truly needs them.
- Prefer read-only permissions by default.
- Document why a new workflow exists.
- Check workflow results before merging changes that affect automation.

## When to update the check

Update `.github/workflows/docs-check.yml` when a new documentation file becomes part of the repository baseline.
