# 2026-11-04 — Replace unavailable contact mailbox

- File: content/en/contact.md.
- Request/source: user in Codex chat explicitly supplied ranka.sro@gmail.com as the current company contact.
- Decision: replace the public rio@ranka.mobi label and mailto target because ranka.mobi has no mail DNS. Keep signed-in private messaging unchanged.
- Verification: build Hugo, inspect generated mailto, publish only the contact page with a backup and compare the public result.
