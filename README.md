# Dormotech email signature

A one-page generator for the company email signature in Outlook. Anyone on the team fills in their details and copies the result.

**Live:** https://andriiloginov.github.io/dormotech-signature/

## What's here
- `index.html` — the generator (no build step, no dependencies).
- `logo.png` — the Dormotech lockup (690 × 168, shown at 230 × 56). Signatures link to this file, so keep the name and location stable.

## How the signature works
- Logo image on the left, a thin mint divider, then name, title, cell, email, dormotech.com and an optional "Book a meeting →" link.
- Text is live HTML in Instrument Sans (Outlook falls back to Arial).
- The logo URL is built from the page address, so it always points at the hosted `logo.png`.

## Using it
1. Fill in your details.
2. **Copy for Outlook** → paste into Outlook (new / web / Mac) signature settings.
3. Classic Outlook for Windows: **Download signature file** → put `Dormotech.htm` into `%APPDATA%\Microsoft\Signatures`.
4. **Copy to Figma** pastes the signature as editable vectors and text.

## Updating
Edit `index.html`, commit and push to `main`. GitHub Pages republishes in about a minute.
Replacing `logo.png` updates the logo in every signature already in use.
