---
title: Obligor Glance Privacy Policy
permalink: /privacy/
---

# Obligor Glance: Privacy Policy

_Last updated: 2 October 2026_

Obligor Glance is a browser extension that identifies the company behind the website you are viewing and shows sanctions, export-control, debarment and country-risk information about it.

## What the extension reads
When you open a website (http/https), the extension reads **identity clues from that page**: the page title, site name, structured data, copyright and footer lines, registration and LEI numbers, phone country codes, and a short sample of visible text. It skips search engines, social networks and webmail. It does not read form fields, passwords, cookies, browsing history or the content of other tabs.

## What stays on your device
- The company memory, the website→company links you confirm, your watchlist and the activity log are stored **only in your browser** (IndexedDB / extension storage).
- Settings, including an optional Anthropic API key, are stored locally in extension storage.
- Nothing about you or your browsing is sent to the publisher of Obligor Glance. Your confirmations are shared only if you opt in (below).

## What is sent to third parties, and when
| Recipient | What | When |
|---|---|---|
| GLEIF (api.gleif.org) | Company names and LEIs to look up | When the extension can't identify a site from its own memory, and in background learning (registry pages by country, ownership links) |
| Anthropic (api.anthropic.com) | The page clues and text sample above | **Only if you add your own API key**, and only when rules can't identify the company |
| The data feed (by default itsjustcharlieinnit.github.io, or your own URL) | A request for the latest data files, with no information about you or your browsing | Every 6 hours |
| The shared-memory server (by default the publisher's Supabase project, or your own) | **Every 6 hours:** a request to download the list of verified website→company links. It contains no information about you or your browsing. **Only if you tick "Share my confirmations":** when you click *Confirm*, *This one* or *Wrong company?*, the website domain, the company ID/name/country/LEI, your vote, a salted hash of a random install ID, and an optional hashed team code | Download: always. Votes: **opt-in only** |

The extension never asks the shared-memory server about the site you are viewing. It downloads the full list of verified links, so the server cannot see your browsing.

## What we don't do
No analytics, advertising, tracking pixels, fingerprinting or sale of data. No remote code is executed.

## Retention and deletion
Local data stays until you remove the extension or use **Settings → Reset memory**. The activity log keeps 90 days. Shared-memory votes are kept until the server operator deletes them. Contact the operator to request deletion of votes tied to your install.

## Contact
Questions: the publisher contact listed on the Chrome Web Store page.
