# Investor Search for Cursor

Build a sourced list of the investors in a market — family offices, VCs, PE firms and
angels — and say honestly how complete it is.

By **BCP partners GmbH** · [bcpp.io](https://www.bcpp.io)

## Install

In Cursor: **Customize → Plugins → From GitHub Repository**, then paste this repository's URL.

To try it before publishing, copy this folder into `~/.cursor/plugins/local/`.

## What it does

Ask for the investors in a country, region or sector. You get one Excel file in which each
field records the page it came from.

It works to tell real investors apart from the advisers who sell to them, asks for proof
before treating two entries as the same firm, searches until six rounds in a row find
nothing new, and keeps its working files so a second run continues instead of repeating.

Where it cannot verify something, it records that rather than filling the gap.

## What it needs

A way to search the web, a way to fetch a page, and a terminal that can run `python3`.
No account, no API key, no database.

Research only — not investment advice.

## Layout

| Path | Read by |
|---|---|
| `.cursor-plugin/plugin.json` | Cursor, as a plugin |
| `skills/investor-search/` | Cursor |
| `.agents/skills/investor-search/` | Cursor, and any agent that reads `.agents/skills` |

The two skill folders are kept byte-for-byte identical. Any change goes into both.

## Other agents

The same skill is packaged separately for each agent it runs in. See
[bcpp.io](https://www.bcpp.io).

## Licence

MIT-0. See LICENSE.

---

© 2026 BCP partners GmbH · [Privacy](https://www.bcpp.io/investor-search-privacy) · [Terms](https://www.bcpp.io/terms-and-conditions)
