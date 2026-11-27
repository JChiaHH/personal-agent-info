# personal-agent-info

Public pages for a private, single-user research & schedule assistant.

| Page | Link |
|---|---|
| **Research Desk dashboard** (encrypted) | https://jchiahh.github.io/personal-agent-info/dash/ |
| Home page | https://jchiahh.github.io/personal-agent-info/ |
| Privacy policy | https://jchiahh.github.io/personal-agent-info/privacy.html |

## Research Desk dashboard
A weekly, curated list of research papers with code, venue ("Published in …"), institutions, senior author,
a transparent quality estimate and evidence (real-world tests, baselines), plus search, filters and CSV export.

**Access:** the page asks for a passphrase. Colleagues: ask the owner for the team passphrase. Without one the
page shows nothing.

**How the data is protected**
- All content is encrypted (AES-256-GCM; the key is derived from the passphrase with PBKDF2-SHA256, 600,000
  rounds) and is only ever decrypted inside your own browser. This repository and GitHub Pages store only
  ciphertext.
- The page loads nothing from other sites, sets no cookies and has no analytics.
- Changing a passphrase revokes access: every update replaces this repository's history with a single fresh
  commit, so old encrypted snapshots are not kept.
- Locks itself after 10 minutes in a background tab (owner view) or with the Lock button.

## Notes
- This repository is updated automatically by the assistant (about twice a day). Its history is rewritten on
  every update: please don't open pull requests or push here.
- The home and privacy pages also serve as the app information for the assistant's Google sign-in.
