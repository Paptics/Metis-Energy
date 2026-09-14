# Metis Energy × Aptics — Gunsynd Solar Farm dashboard

Private, gated client proposal page for Metis Energy (Gunsynd Solar Farm — facility code `GUSF`, QLD),
built from the Aptics dashboard-kit base template.

## Files

- `index.html` — the proposal page (self-contained: styles and script are inline)
- `assets/` — the four images the page references (`thermal-01.png`, `thermal-02.png`, `mc4-01.png`, `mc4-04.png`)
- `.nojekyll` — required so GitHub Pages serves the files as-is instead of running Jekyll processing over them

## Publish (GitHub Pages)

1. Push these three items to the root of a private GitHub repo named for the client/site.
2. Repo **Settings → Pages → Build and deployment → Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site publishes at `https://<org>.github.io/<repo>/`.
4. Share the gated link as `https://<org>.github.io/<repo>/?key=<the access key>` — get the current key
   from Phillip rather than committing it here; it should never sit in plaintext in this repo or in the
   page's own source (the page only ever stores a salted hash of it).
5. Open the `?key=` link yourself and read the live page end to end before it goes to the client.

## Access gate

The page is gated by work-email domain (auto-fills the key for `metisenergy.com` / `aptics.com` addresses)
or by a direct `?key=` link. Regenerating the gate (new client, new key) means producing a fresh salt,
SHA-256 hash, and base64-encoded key — see `PROMPT.md` / `PLAYBOOK.md` in the Aptics dashboard-kit Drive
folder for the full process.

## Status

Built 14 September 2026. Content, facts and sourcing are documented in the change list delivered alongside
this repo — flagged figures should be re-confirmed before this goes live to the client.
