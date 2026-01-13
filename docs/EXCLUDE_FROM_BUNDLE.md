Files to exclude from distribution bundle
=========================================

When creating the ZIP for Gumroad, exclude the following files and directories:

- `.git/` — version control metadata
- `.github/` — CI workflows and actions (not required for buyer bundle)
- `node_modules/` — dependency installations
- `.env.local`, `.env` — local environment files with secrets
- Any backup or personal files (e.g., `notes/`, `drafts/`)

This document is informational; the canonical exclusion list is in `RELEASE_CHECKLIST.md`.
