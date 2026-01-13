Release Checklist for Gumroad Bundle
===================================

Before creating the ZIP to upload to Gumroad, verify the following items:

- Docs completed: `docs/SETUP.md`, `docs/ARCHITECTURE.md`, `docs/DEMO.md`, `docs/LICENSE.md` present and accurate.
- CI passing: Confirm GitHub Actions CI is green on main (optional, helpful for buyers).
- No secrets committed: `.env.local`, `.env`, or other secret files are NOT present in the bundle.
- Version tagged: `VERSION` file exists and matches release tag.
- Demo tested: Run seed and basic manual smoke tests (login, create course, create order).
- ZIP verified: Create a ZIP and test extraction and a fresh `npm ci` + `npm run build` inside the extracted folder.

Files and directories to exclude from the ZIP bundle (do not include these):

- `.git/` directory
- `.github/` directory (CI workflows not required in buyer bundle)
- Any local `node_modules/` directories
- `.env.local`, `.env`, or other local environment files
- Personal notes, drafts, or TODO files (if present)

Optional: Include a `CHANGES.md` or release notes document describing what changed in this version.

Once all checklist items are validated, create a ZIP of the repository root (excluding the items above)
and upload to Gumroad.
