# RPG1 Backups — OAuth application information

This **public** repository contains only the static homepage and privacy-policy
information for a personal Google Drive database-backup utility.

**The actual RPG1 game-development source, databases, test results and Google
OAuth credentials are NOT kept in this repository.** The RPG1 development
repository is private.

## Site files

- [index.html](index.html) — public application homepage.
- [privacy.html](privacy.html) — public privacy policy.

## Publish through GitHub Pages

In this repository, open **Settings → Pages** and choose:

- **Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/(root)`

Click **Save**, then wait until GitHub reports the published website address.
Expected project-site pattern:

- Homepage: `https://dickwork.github.io/rpg1-backup-oauth/`
- Privacy: `https://dickwork.github.io/rpg1-backup-oauth/privacy.html`

**Do not put these URLs into Google Cloud until both are actually live.**
Google's OAuth branding and verification process may require proof of domain
ownership. A shared `github.io` hostname is **not guaranteed** to be accepted
as a verified domain; in that case, use a domain you control instead.

## Backup implementation state

The pages describe the utility's intended operating model. Google Drive OAuth
authorization, first off-machine backup upload, restore verification and
unattended nightly timer have **not yet been completed**. Revise the privacy
policy if the implemented access scope or data handling differs.

Never commit credentials, tokens, private data or SQLite backups here.
